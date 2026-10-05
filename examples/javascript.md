# JavaScript example

```js
const response = await fetch("https://genory.dev/api/profile", {
  method: "POST",
  headers: {
    "Authorization": `Bearer ${process.env.GENORY_API_KEY}`,
    "Content-Type": "application/json",
  },
  body: JSON.stringify({
    country: "DE",
    amount: 1,
    fields: ["firstName", "lastName", "email"],
  }),
});

if (!response.ok) {
  throw new Error(`Genory request failed: ${response.status}`);
}

const data = await response.json();
console.log(data);
```

Keep API keys in environment variables and follow the current documentation at https://genory.dev/docs.
