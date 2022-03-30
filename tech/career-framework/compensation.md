# Compensation

We don't have exact salary bands, we define **lower bounds** based on your [career track](career-tracks/readme.md) and [grade](grades.md). The main purpose of the lower bounds is to ensure **fairness** across whole tech team and that nobody is underpaid. And as you get better, it also ensures that getting a raise is **guaranteed**. So at the moment, it's mainly an "alerting" mechanism for managers rather than a magic formula that determines the exact salary, especially because we acknowledge that the competencies do not capture full spectrum of stuff that everyone does.

## Normalization

The minimum salary is expressed in a normalized form, which is a monthly salary in Czech Republic in CZK. That is what majority of our team "thinks in", however we are a global company, employing people in multiple countries, paying in different currencies and offering different types of salaries (hourly rate, monthly, annual). So in order to convert between salary and normalized salary use the following formulas:

- `normalized = salary × period × currency × country`
- **`salary = normalized / (period × currency × country)`**

Besides salary or normalized salary, the formulas contain three multipliers. Use the following values based on your salary period, currency and country. How to do that in practice is described in the examples section below.

| Period | Currency | Country |
|--------|----------|---------|
| **Hour** - 160<br/> **Month** - 1 <br/>**Year** - 0.0833 | **CZK** - 1<br/> **EUR** - 26<br/> **GBP** - 30<br/> **USD** - 22 | **CZ** - 1.00<br/> **UK** - 0.60<br/> **NL** - 0.55<br/> **DE** - 0.55<br/> **BE** - 0.55<br/> **FR** - 0.65<br/> **ES** - 0.75<br/> **US** - 0.50<br/> **NO** - 0.55<br/> **PL** - 1.00 |

## Examples

Let's assume an engineer with progress P = 1.80. Here are sample details of that career track and grade from the [grading overview](grades.md):

| Track    | Min P | Max P | Grade | Job Title                | Min Salary | Next Salary |
|----------|-------|-------|-------|--------------------------|------------|-------------|
| Engineer | 1.20  | 2.40  | IC3   | {Discriminator} Engineer | 69000      | 98000       |

What would be the minimum salary for such engineer?

- Czech employee with monthly salary in CZK: 69000 / (1 × 1 × 1) = **69000 CZK monthly**
- Czech contractor with hourly rate in CZK: 69000 / (160 × 1 × 1) = **431 CZK hourly**
- British employee with annual salary in GBP: 69000 / (0.0833 × 30 × 0.60) = **46018 GBP annually**
- German employee with annual salary in EUR: 69000 / (0.0833 × 26 × 0.55) = **57925 EUR annually**

## Next Salary

We acknowledge that it takes long time to increase overall progress e.g. for an engineer from 1.20 above 2.40 it might take a few years. That doesn't mean there should be no raise during that period, managers are reviewing compensation much more frequently, at least every 6 months. Plus they're taking other factors into account. In order to capture this, we use min progress (`x0`), max progress (`x1`), min salary (`y0`) and next salary (`y1`) and look at the linear interpolation of min salary (`y`) based on exact progress (`x`). 

<img alt="Salary interpolation" height="200px" src="https://user-images.githubusercontent.com/435787/131226550-929f09fa-0272-45de-b9f2-fa3d7df6e321.png">

So if the progress of an engineer is 1.80, which is right between min progress (1.20) and max progress (2.40), their salary should be somewhere around the midpoint of min salary (69000) and next salary (98000), which is 83500. This is used just as an **indicator**, this is not a guarantee. However it allows us to progressively raise salary fairly, even if grades don't change for longer periods of time. On the other hand, we are not giving a raise with every single 0.1 increment in progress. The rule of thumb we use: if salary of a person gets lower than 90% of the interpolation (`y`) thanks the their increased progress (`x`), we consider to give a raise the person. So following up on the example above, an engineer with salary 69000 and progress 1.80 is at **cca 83% of the interpolated salary 83500**. Therefore we'd align them with the interpolated salary and give them a raise. 
