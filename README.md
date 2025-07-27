# 🇨🇦 Canada Provinces and Cities Dataset

An open dataset listing all **Canadian provinces and territories**, along with their **major cities**, organized in a clean and developer-friendly JSON structure.

Ideal for address validation, dropdowns, logistics apps, location services, and civic tech projects.

---

## 🗂 Data Format

The main dataset is provided in nested JSON format like this:

```json
[
  {
    "province": "Ontario",
    "cities": ["Toronto", "Ottawa", "Mississauga", "Hamilton", "London"]
  },
  {
    "province": "British Columbia",
    "cities": ["Vancouver", "Victoria", "Surrey", "Burnaby"]
  }
]
```

---



## 🔍 Sample Usage

### ✅ JavaScript – List All Cities (Node.js)

```js
const fs = require("fs");

const data = JSON.parse(
  fs.readFileSync("data/canada-provinces-cities.json", "utf8")
);

data.forEach((province) => {
  province.cities.forEach((city) => {
    console.log(`${province.province} → ${city}`);
  });
});
```

---

## 🔧 Use Cases

- 📍 Province and city dropdowns
- 📋 Address validation forms
- 🚛 E-commerce shipping and delivery platforms
- 📊 Dashboards and filters
- 🌎 Location-aware services and maps

---

## 📜 License

- **Data**: Licensed under [Open Data Commons Attribution License v1.0](https://opendatacommons.org/licenses/by/1-0/)
- **Scripts**: Licensed under the [MIT License](LICENSE-MIT.txt)

---

## 🤝 Contributing

Contributions are welcome!

1. Fork this repo
2. Create a new branch
3. Make your changes
4. Submit a Pull Request
