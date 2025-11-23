## 📈 High-Growth Industry Trends: Unicorn Analysis

Did you know that the **average return from investing in stocks is 10% per year** (not accounting for inflation)? But who wants to be *average*?!

We are going to support an **investment firm** by analyzing trends in **high-growth companies**. They are interested in identifying:

- Which **industries** are producing the **highest valuations**
- The **rate at which new high-value companies** (unicorns) are emerging

By providing this information, we'll give them a **competitive insight** into industry trends and help inform **portfolio strategy** moving forward.

---

## 🦄 Unicorns Database Structure

Here is the unicorns database, which includes the following tables:

### `dates`

| Column        | Description                                      |
|---------------|--------------------------------------------------|
| company_id    | A unique ID for the company                      |
| date_joined   | The date the company became a unicorn            |
| year_founded  | The year the company was founded                 |

---

### `funding`

| Column          | Description                                      |
|------------------|--------------------------------------------------|
| company_id       | A unique ID for the company                      |
| valuation        | Company value in US dollars                      |
| funding          | Amount of funding raised in US dollars           |
| select_investors | List of key investors in the company             |

---

### `industries`

| Column      | Description                                      |
|-------------|--------------------------------------------------|
| company_id  | A unique ID for the company                      |
| industry    | The industry the company operates in             |

---

### `companies`

| Column      | Description                                      |
|-------------|--------------------------------------------------|
| company_id  | A unique ID for the company                      |
| company     | Name of the company                              |
| city        | City where the company is headquartered          |
| country     | Country where the company is headquartered       |
| continent   | Continent where the company is headquartered     |

---

## 🧾 Expected Output

The final query should return a table in the following format:

| industry   | year | num_unicorns | average_valuation_billions |
|------------|------|--------------|-----------------------------|
| industry1  | 2021 | ---          | ---                         |
| industry2  | 2020 | ---          | ---                         |
| industry3  | 2019 | ---          | ---                         |
| industry1  | 2021 | ---          | ---                         |
| industry2  | 2020 | ---          | ---                         |
| industry3  | 2019 | ---          | ---                         |
| industry1  | 2021 | ---          | ---                         |
| industry2  | 2020 | ---          | ---                         |
| industry3  | 2019 | ---          | ---                         |

Where `industry1`, `industry2`, and `industry3` represent the **top 3 performing industries**.
