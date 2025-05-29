# Power BI Business Insights 360 II

## Project Overview
The [Codebasics](https://codebasics.io/) [Data Analytics Bootcamp](https://codebasics.io/bootcamps/data-analytics-bootcamp-with-practical-job-assistance) exhibits a fictional company called AtliQ Technologies. AtliQ was rapidly proliferating to various markets around the world. However, AtliQ relied on Excel files for their data analytics needs. Since AtliQ's data was spread across multiple large tables (some containing over a million records), analyzing them in Excel was cumbersome. Moreover, stakeholders found that static reports produced from Excel pivot tables were difficult and time-consuming to digest. This weakened data anaytics capability hindered AtliQ's success when they attempted to expand to markets in Latin America.

The objective of this project is to create a Power BI dashboard which stakeholders from various business verticals (**finance**, **sales**, **marketing**, **supply chain**, and **executive**) can use to effectively and efficiently gather insights from data to help inform important company decisions. The interactive and visual nature of Power BI dashboards should help stakeholders better interpret the data with less time compared to static reports produced in Excel.

This README file provides some business context about the fictional company AtliQ Technologies, as well as a brief high-level technical overview of the project.


## 📊 Interactive Dashboard on Power BI Service
Click the link below to explore the live, interactive dashboard on Power BI Service:<br>
[🔗 **View Dashboard**](https://app.powerbi.com/view?r=eyJrIjoiN2JkNjFkYWEtZGJjNi00MTAwLTg4NjEtOTAyMjFjZmM4ZGZlIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9&pageName=c560809d0bd55033207c)
<br>



## AtliQ Technologies Business Model

<details>
  <summary><b>Overview</b></summary>

AtliQ manufactures computer hardware **products** (e.g., mouse, keyboard, printer, monitor) and then sells them to various **customers** which are stores such as Amazon and Best Buy. Hence, AtliQ's customers are in the form of <ins>store businesses</ins> (e.g., Amazon, Best Buy) and should not be confused with customers in the form of people (i.e., the people purchasing products from Amazon or Best Buy).

<br>
</details>

<details>
  <summary><b>Customers</b></summary>

AtliQ's customers are categorized into two different **platforms**:
1. Brick & Motar
   * stores that have physical location(s)
2. E-Commerce
   * stores which only sell products online
<br>

AtliQ's customers are categorized into three different **channels**:
1. Retailer
   * Stores not owned by AtliQ (e.g. Amazon, Best Buy)
3. Direct
   * Stores owned by AtliQ. These are AltiQ Exclusive and AtliQ E-Store.
5. Distributor
   * Some markets have laws/regulations which only allow AtliQ to sell products to a distributor type customer within that market. AtliQ sells products to the distributor; the distributor then sells the products to various stores within that market.

<br>
</details>

<details>
  <summary><b>Profit and Loss (P&L) Statement</b></summary>

This simplified P&L statement should give a better understanding of AtliQ's business model. In this example, the P&L values are derived from one sale transaction of one product being sold to one customer.
| P&L Line Item | Description | P&L Value Formula | P&L Value Calculation | Final P&L Value |
| :- | :- | :- | :- | -: |
| Gross Price |  The base price of a product | not applicable | `not applicable` | `$50.00` |
| Pre-Invoice Deduction | For every fiscal year, the sales team determines a<br>pre-invoice deduction percentage for each<br><ins>specific customer</ins>. The pre-invoice deduction<br>percentage is based on AtliQ's relationship and<br>experience with the customer. The pre-invoice<br>deduction is applied to the gross price of the<br>product before it is billed to the customer. In this<br>example, the customer receives a pre-invoice<br>deduction of 10% of gross price. | (Gross Price $) *<br> (Pre&nbsp;Invoice&nbsp;Deduction&nbsp;%) | `$50.00` *<br>`0.10` | `$5.00` |
| Net Invoice Sales | The amount of money that is billed to the<br>customer to obtain the product, after<br>pre-invoice deductions are subtracted<br>from gross price. | (Gross Price $) -<br>(Pre&nbsp;Invoice Deduction $) | `$50.00` -<br>`$5.00` | `$45.00` |
| Post-Invoice Deudctions | For&nbsp;each&nbsp;calendar&nbsp;month,&nbsp;the&nbsp;sales&nbsp;team<br>determines&nbsp;a&nbsp;post-invoice&nbsp;deduction&nbsp;percentage<br>based&nbsp;on&nbsp;a&nbsp;<ins>specific&nbsp;customer&nbsp;and&nbsp;product</ins>.&nbsp;For<br>example,&nbsp;if&nbsp;AtliQ&nbsp;sells&nbsp;a&nbsp;product&nbsp;to&nbsp;a&nbsp;customer<br>and&nbsp;that&nbsp;customer&nbsp;agrees&nbsp;to&nbsp;display&nbsp;the&nbsp;product&nbsp;at<br>a&nbsp;prime&nbsp;location&nbsp;within&nbsp;the&nbsp;store&nbsp;during&nbsp;a<br>specific&nbsp;calendar&nbsp;month,&nbsp;AtliQ&nbsp;may&nbsp;pay&nbsp;that<br>customer&nbsp;a&nbsp;post-invoice&nbsp;deduction.&nbsp;AtliQ&nbsp;pays&nbsp;a<br>post-invoice&nbsp;deduction&nbsp;amount&nbsp;as&nbsp;a&nbsp;rebate&nbsp;to&nbsp;the<br>customer&nbsp;after&nbsp;net&nbsp;invoice&nbsp;sales.&nbsp;In&nbsp;this&nbsp;example,<br>the&nbsp;customer&nbsp;receives&nbsp;a&nbsp;post-invoice&nbsp;deduction&nbsp;of<br>20%&nbsp;of&nbsp;net&nbsp;invoice&nbsp;sales. | (Net Invoice Sales $) *<br>(Post-Invoice Deduction %) | `$45.00` *<br>`0.20` | `$9.00` |
| Net Sales | Revenue | (Net Invoice Sales $) -<br>(Post-Invoice Deudctions $) | `$45.00` -<br>`$9.00` | `$36.00` |
| Cost of Goods Sold (COGS) | Expenses AtliQ incurs such as manufacturing<br>products, shipping products, and storing products<br>in warehouses. | (Manufacturing Cost $) +<br>(Freight Cost $) +<br>(Other COGS $) | `$9.00` +<br>`$4.00` +<br>`$3.00` | `$16.00` |
| Gross Margin | AtliQ's Profit after deducing COGS from Net Sales. | (Net Sales $) -<br>(COGS $) | `$36.00` -<br>`$16.00` | `$20.00` |
| Operational Expenses | Expenses AtliQ incurs from activities such as<br>advertising and promotions of products<br>performed by the marketing team. | (Ads & Promotions $) +<br>(Other&nbsp;Operational&nbsp;Expense&nbsp;$) | `$10.00` +<br>`$5.00` | `$15.00` |
| Net Profit | AtliQ's Profit after deducting operational expenses<br>from gross margin. | (Gross Margin $) -<br>(Operational Expenses $) | `$20.00` -<br>`$15.00` | `$5.00` |

<br>
</details>


<details>
  <summary><b>AtliQ Fiscal Dates</b></summary>

AtliQ's fiscal year begins in September and ends in August the following year. The example below shows AtliQ's fiscal dates for fiscal year 2021 compared to calendar dates.
| 	Calendar Month and Year	 | 	AtliQ Fiscal Year	 | 	AtliQ Fiscal Month Number | 	AtliQ Fiscal Quarter	 |
| 	-:	 | 	-:	 | 	-:	 | 	-:	 |
| 	September 2020	 | 	2021	 | 	1	 | 	Q1	 |
| 	October 2020	 | 	2021	 | 	2	 | 	Q1	 |
| 	November 2020	 | 	2021	 | 	3	 | 	Q1	 |
| 	December 2020	 | 	2021	 | 	4	 | 	Q2	 |
| 	January 2021	 | 	2021	 | 	5	 | 	Q2	 |
| 	February 2021	 | 	2021	 | 	6	 | 	Q2	 |
| 	March 2021	 | 	2021	 | 	7	 | 	Q3	 |
| 	April 2021	 | 	2021	 | 	8	 | 	Q3	 |
| 	May 2021	 | 	2021	 | 	9	 | 	Q3	 |
| 	June 2021	 | 	2021	 | 	10	 | 	Q4	 |
| 	July 2021	 | 	2021	 | 	11	 | 	Q4	 |
| 	August 2021	 | 	2021	 | 	12	 | 	Q4	 |

<br>
</details>




## Data Sources

<details>
  <summary><b>Dimension Tables</b></summary>

AtliQ's data engineers prepared various dimension tables and stored them in a MySQL database schema. Sample records from each dimension table are provided below.

<br>

**dim_market**
| market | sub_zone | region |
| :- | :- | :- |
| Japan | ROA | APAC |
| Sweden | NE | EU |
| Brazil | LATAM | LATAM |

Notes:
* `market` is a primary key field.

<br>

**dim_customer**
| customer_code | customer         | market       | platform        | channel    |
|:--------------|:-----------------|:-------------|:-----------------|:-----------|
| 90022082      | Amazon           | USA          | E-Commerce       | Retailer   |
| 90023030      | Amazon           | Canada       | E-Commerce       | Retailer   |
| 90004068      | Amazon           | Japan        | E-Commerce       | Retailer   |
| 90006156      | Amazon           | Philiphines  | E-Commerce       | Retailer   |
| 90007197      | Amazon           | South Korea  | E-Commerce       | Retailer   |
| 70022085      | Atliq e Store    | USA          | E-Commerce       | Direct     |
| 70023032      | Atliq e Store    | Canada       | E-Commerce       | Direct     |
| 70004070      | Atliq e Store    | Japan        | E-Commerce       | Direct     |
| 70006158      | Atliq e Store    | Philiphines  | E-Commerce       | Direct     |
| 70007199      | Atliq e Store    | South Korea  | E-Commerce       | Direct     |
| 70022084      | AltiQ Exclusive  | USA          | Brick & Mortar   | Direct     |
| 70023031      | AltiQ Exclusive  | Canada       | Brick & Mortar   | Direct     |
| 70004069      | AltiQ Exclusive  | Japan        | Brick & Mortar   | Direct     |
| 70006157      | AltiQ Exclusive  | Philiphines  | Brick & Mortar   | Direct     |
| 70007198      | AltiQ Exclusive  | South Korea  | Brick & Mortar   | Direct     |
| 90022078      | Costco           | USA          | Brick & Mortar   | Retailer   |
| 90023027      | Costco           | Canada       | Brick & Mortar   | Retailer   |
| 90022080      | Staples          | USA          | Brick & Mortar   | Retailer   |
| 90023029      | Staples          | Canada       | Brick & Mortar   | Retailer   |
| 80001019      | Neptune          | China        | Brick & Mortar   | Distributor|
| 80006154      | Synthetic        | Philiphines  | Brick & Mortar   | Distributor|

Notes:
* `customer_code` is a primary key field. 

<br>

**dim_product**
| product_code  | division | segment     | category                     | product           | variant        |
|:--------------|:---------|:------------|:-----------------------------|:------------------|:---------------|
| A0721150401   | P & A    | Peripherals | Graphic Card                 | AQ GT 21          | Standard       |
| A0721150402   | P & A    | Peripherals | Graphic Card                 | AQ GT 21          | Plus 1         |
| A0721150403   | P & A    | Peripherals | Graphic Card                 | AQ GT 21          | Plus 2         |
| A0721150404   | P & A    | Peripherals | Graphic Card                 | AQ GT 21          | Premium        |
| A3119150301   | P & A    | Accessories | Keyboard                     | AQ Gamers         | Standard 1     |
| A3119150302   | P & A    | Accessories | Keyboard                     | AQ Gamers         | Standard 2     |
| A3119150303   | P & A    | Accessories | Keyboard                     | AQ Gamers         | Plus 1         |
| A3120150304   | P & A    | Accessories | Keyboard                     | AQ Gamers         | Plus 2         |
| A3120150305   | P & A    | Accessories | Keyboard                     | AQ Gamers         | Premium 1      |
| A3120150306   | P & A    | Accessories | Keyboard                     | AQ Gamers         | Premium 2      |
| A4118110101   | PC       | Notebook    | Personal Laptop              | AQ Aspiron        | Standard Grey  |
| A4118110102   | PC       | Notebook    | Personal Laptop              | AQ Aspiron        | Standard Blue  |
| A4118110103   | PC       | Notebook    | Personal Laptop              | AQ Aspiron        | Standard Red   |
| A4118110104   | PC       | Notebook    | Personal Laptop              | AQ Aspiron        | Plus Grey      |
| A4118110105   | PC       | Notebook    | Personal Laptop              | AQ Aspiron        | Plus Blue      |
| A4118110106   | PC       | Notebook    | Personal Laptop              | AQ Aspiron        | Plus Red       |
| A4118110107   | PC       | Notebook    | Personal Laptop              | AQ Aspiron        | Premium Black  |
| A6419160301   | N & S    | Storage     | External Solid State Drives  | AQ Clx1           | Standard       |
| A6419160302   | N & S    | Storage     | External Solid State Drives  | AQ Clx1           | Plus           |
| A6419160303   | N & S    | Storage     | External Solid State Drives  | AQ Clx1           | Premium        |
| A7118160101   | N & S    | Networking  | Wi fi extender               | AQ Wi Power Dx1   | Standard       |
| A7119160102   | N & S    | Networking  | Wi fi extender               | AQ Wi Power Dx1   | Plus           |
| A7119160103   | N & S    | Networking  | Wi fi extender               | AQ Wi Power Dx1   | Premium        |

Notes:
* `product_code` is a primary key field.

<br>

</details>


<details>
  <summary><b>Fact Tables</b></summary>

AtliQ's data engineers prepared various fact tables and stored them in a MySQL database schema. Sample records from each fact table are provided below.

<br>

**fact_forecast_monthly**
| date       | product_code  | division | category                   | product     | customer_code | customer_name         | market    | platform      | channel  | forecast_quantity |
|-----------:|:--------------|:---------|:---------------------------|:------------|:--------------|:----------------------|:----------|:--------------|:---------|------------------:|
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 70008169      | AltiQ Exclusive       | Australia | Brick & Mortar| Direct   | 318               |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90008165      | Forward Stores        | Australia | Brick & Mortar| Retailer | 69                |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90008166      | Sound                 | Australia | Brick & Mortar| Retailer | 269               |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90008167      | Electricalsocity      | Australia | Brick & Mortar| Retailer | 215               |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 70008170      | Atliq e Store         | Australia | E-Commerce    | Direct   | 504               |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020097      | Atlas Stores          | Austria   | Brick & Mortar| Retailer | 7                 |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020098      | Electricalsquipo Stores| Austria   | Brick & Mortar| Retailer | 2                 |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020099      | Integration Stores    | Austria   | Brick & Mortar| Retailer | 2                 |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020101      | Euronics              | Austria   | Brick & Mortar| Retailer | 3                 |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020102      | Fnac-Darty            | Austria   | Brick & Mortar| Retailer | 7                 |

Notes:
* This table contains data on the forecasted quantity of sold products for specific customers, on a monthly level
* The data engineer provided this table in **denormalized** format
* The columns `date`, `product_code`, and `customer_code` make up a **composite primary key**
* Data for monthly forecast of quantity of products sold is available from the beginning of fiscal year 2018 to the end of fiscal year 2022 (September 2017 - August 2022)

<br>

**fact_sales_monthly**
| date       | product_code  | division | category                   | product     | customer_code | customer_name         | market    | platform      | channel  | sold_quantity |
|-----------:|:--------------|:---------|:---------------------------|:------------|:--------------|:----------------------|:----------|:--------------|:---------|--------------:|
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 70008169      | AltiQ Exclusive       | Australia | Brick & Mortar| Direct   | 158           |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90008165      | Forward Stores        | Australia | Brick & Mortar| Retailer | 348           |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90008166      | Sound                 | Australia | Brick & Mortar| Retailer | 243           |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90008167      | Electricalsocity      | Australia | Brick & Mortar| Retailer | 261           |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 70008170      | Atliq e Store         | Australia | E-Commerce    | Direct   | 138           |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020097      | Atlas Stores          | Austria   | Brick & Mortar| Retailer | 2             |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020098      | Electricalsquipo Stores| Austria   | Brick & Mortar| Retailer | 6             |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020099      | Integration Stores    | Austria   | Brick & Mortar| Retailer | 4             |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020101      | Euronics              | Austria   | Brick & Mortar| Retailer | 3             |
| 2019-09-01 | A6218160101   | N & S    | External Solid State Drives | AQ Digit SSD| 90020102      | Fnac-Darty            | Austria   | Brick & Mortar| Retailer | 6             |

Notes:
* This table contains data on the actual sold quantity of products for specific customers, on a monthly level
* The data engineer provided this table in **denormalized** format
* The columns `date`, `product_code`, and `customer_code` make up a **composite primary key**
* Data for monthly quantity of products actually sold is available from the beginning of fiscal year 2018 (September 2017) to December 2021

<br>

**freight_cost**
| 	market	 | 	fiscal_year	 | 	freight_pct	 | 	other_cost_pct	 |
| 	:-	 | 	-:	 | 	-:	 | 	-:	 |
| 	Australia	 | 	2018	 | 	0.0188	 | 	0.005	 |
| 	Australia	 | 	2019	 | 	0.0304	 | 	0.0048	 |
| 	Australia	 | 	2020	 | 	0.0254	 | 	0.0043	 |
| 	Australia	 | 	2021	 | 	0.0254	 | 	0.0043	 |
| 	Australia	 | 	2022	 | 	0.0254	 | 	0.0043	 |
| 	Bangladesh	 | 	2018	 | 	0.0219	 | 	0.0058	 |
| 	Bangladesh	 | 	2019	 | 	0.0249	 | 	0.0053	 |
| 	Bangladesh	 | 	2020	 | 	0.0258	 | 	0.0035	 |
| 	Bangladesh	 | 	2021	 | 	0.0258	 | 	0.0035	 |
| 	Bangladesh	 | 	2022	 | 	0.0258	 | 	0.0035	 |

Notes:
* Freight cost is one component of COGS. This table contains data at a fiscal year level on freight cost (as a percentage of net sales) for each specific market.
* The columns `market` and `fiscal_year` make up a **composite primary key**

<br>

**gross_price**
| product_code  | fiscal_year | gross_price |
|:--------------|------------:|------------:|
| A0118150103   | 2018        | 19.363      |
| A0118150103   | 2019        | 19.3442     |
| A0118150103   | 2020        | 22.1317     |
| A0118150103   | 2021        | 21.7795     |
| A0118150103   | 2022        | 23.992      |
| A0118150104   | 2018        | 19.5743     |
| A0118150104   | 2019        | 18.5072     |
| A0118150104   | 2020        | 20.7734     |
| A0118150104   | 2021        | 22.9729     |
| A0118150104   | 2022        | 23.6298     |

Notes:
* Gross price is the base price of a product. This table contains data on the gross price of each specific product on a fiscal year level. 
* The columns `product_code` and `fiscal_year` make up a **composite primary key**

<br>

**manufacturing_cost**
| product_code  | cost_year | manufacturing_cost |
|:--------------|----------:|-------------------:|
| A0118150103   | 2018      | 5.9469             |
| A0118150103   | 2019      | 5.5306             |
| A0118150103   | 2020      | 6.3264             |
| A0118150103   | 2021      | 6.59               |
| A0118150103   | 2022      | 7.1831             |
| A0118150104   | 2018      | 5.8958             |
| A0118150104   | 2019      | 5.4242             |
| A0118150104   | 2020      | 6.4789             |
| A0118150104   | 2021      | 6.8199             |
| A0118150104   | 2022      | 7.3655             |

Notes:
* Manufacturing cost is one component of COGS. This table contains data at a fiscal year level on manufacturing cost ($) for one unit quantity of each specific product.
* The columns `product_code` and `cost_year` make up a **composite primary key**.

<br>

**post_invoice_deductions**
| customer_code | product_code   | date       | discounts_pct | other_deductions_pct |
|:--------------|:---------------|-----------:|--------------:|---------------------:|
| 70002017      | A0118150103    | 2021-09-01 | 0.284819951   | 0.070015705          |
| 70002017      | A0118150103    | 2021-10-01 | 0.221476421   | 0.097933181          |
| 70002017      | A0118150104    | 2021-09-01 | 0.243071646   | 0.071690918          |
| 70002017      | A0118150104    | 2021-10-01 | 0.280381778   | 0.099631078          |
| 70002017      | A0219150201    | 2021-09-01 | 0.256135122   | 0.066692363          |
| 70002017      | A0219150201    | 2021-10-01 | 0.268149981   | 0.077287177          |

Notes:
* This table contains data on post-invoice deductions (as a percentage of net invoice sales) of a product for a specific customer, on a monthly level.
* The columns `customer_code`, `product_code` and `date` make up a **composite primary key**.

<br>

**pre_invoice_deductions**
| customer_code | fiscal_year | pre_invoice_discount_pct |
|:--------------|------------:|--------------------------:|
| 70002017      | 2018        | 0.0824421975              |
| 70002017      | 2019        | 0.0776586135              |
| 70002017      | 2020        | 0.0734578107              |
| 70002017      | 2021        | 0.0702694757              |
| 70002017      | 2022        | 0.1056778298              |
| 70002018      | 2018        | 0.2955677085              |
| 70002018      | 2019        | 0.2576548034              |
| 70002018      | 2020        | 0.2254809791              |
| 70002018      | 2021        | 0.2061071236              |
| 70002018      | 2022        | 0.2930927104              |

Notes:
* This table contains data on pre-invoice deductions (as a percentage of gross price) for each specific customer, on a fiscal year level.
* The columns `customer_code`, and `fiscal_year` make up a **composite primary key**.

<br>

</details>


<details>
  <summary><b>Additional Data Tables</b></summary>

Additional data tables were provided in stakeholder meetings. Sample records from each table are provided below.

<br>

**operational_expenses**
| 	market	 | 	fiscal_year	 | 	ads_promotions_pct	 | 	other_operational_expense_pct	 |
| 	:-	 | 	-:	 | 	-:	 | 	-:	 |
| 	Brazil	 | 	2018	 | 	0.11178	 | 	0.17172	 |
| 	Brazil	 | 	2019	 | 	0.156975	 | 	0.21147	 |
| 	Brazil	 | 	2020	 | 	0.14214	 | 	0.185606	 |
| 	Brazil	 | 	2021	 | 	0.1451875	 | 	0.203414	 |
| 	Brazil	 | 	2022	 | 	0.18952	 | 	0.196524	 |
| 	Canada	 | 	2018	 | 	0.141264	 | 	0.363528	 |
| 	Canada	 | 	2019	 | 	0.125895	 | 	0.27489	 |
| 	Canada	 | 	2020	 | 	0.101043	 | 	0.231132	 |
| 	Canada	 | 	2021	 | 	0.143117	 | 	0.283305	 |
| 	Canada	 | 	2022	 | 	0.314356	 | 	0.365959	 |

Notes:
* Provided in .csv format
* This table contains data on operational expenses (as a percentage of net sales) for each specific market, on a fiscal year level.
* The columns `market`, and `fiscal_year` make up a **composite primary key**.

<br>

**targets**
| 	market	 | 	month	 | 	ns_target	 | 	gm_target	 | 	np_target	 |
| 	:-	 | 	-:	 | 	-:	 | 	-:	 | 	-:	 |
| 	France	 | 	9/1/2021	 | 	$10,198,819.89	 | 	$3,346,388.95	 | 	-$725,768.42	 |
| 	France	 | 	10/1/2021	 | 	$15,549,771.95	 | 	$4,403,518.54	 | 	-$1,422,866.33	 |
| 	France	 | 	11/1/2021	 | 	$15,904,636.14	 | 	$6,218,833.51	 | 	-$916,393.33	 |
| 	France	 | 	12/1/2021	 | 	$17,697,536.05	 | 	$4,805,448.09	 | 	-$1,607,007.06	 |
| 	Indonesia	 | 	9/1/2021	 | 	$8,064,974.87	 | 	$2,796,600.63	 | 	-$1,089,126.47	 |
| 	Indonesia	 | 	10/1/2021	 | 	$10,900,556.90	 | 	$3,853,546.03	 | 	-$1,278,820.63	 |
| 	Indonesia	 | 	11/1/2021	 | 	$11,918,830.63	 | 	$4,232,776.48	 | 	-$1,673,999.76	 |
| 	Indonesia	 | 	12/1/2021	 | 	$12,657,658.69	 | 	$4,186,339.00	 | 	-$2,248,949.51	 |

Notes:
* Provided in .xlsx format
* Target data is only available for fiscal year 2022 and only available for the KPIs: net sales, gross margin, and net profit
* Target data is available for each specific market on a monthly level
* The columns `market`, and `month` make up a **composite primary key**.

<br>

**marketshare**
| 	sub_zone	 | 	category	 | 	fy_desc	 | 	total_market_sales_$	 | 	atliq_sales_$	 | 	dale_sales_$	 | 	innovo_sales_$	 | 	pacer_sales_$	 | 	bp_sales_$	 | 	others_sales_$	 |
| 	:-	 | 	:-	 | 	-:	 | 	-:	 | 	-:	 | 	-:	 | 	-:	 | 	-:	 | 	-:	 | 	-:	 |
| 	LATAM	 | 	Business&nbsp;Laptop	 | 	2019	 | 	1084.4776	 | 	0.286	 | 	255.9367136	 | 	117.7308883	 | 	82.41162178	 | 	57.68813525	 | 	570.4242411	 |
| 	LATAM	 | 	Business Laptop	 | 	2020	 | 	1523.0215	 | 	1.04346	 | 	319.834515	 | 	102.3470448	 | 	84.94804718	 | 	54.24393374	 | 	960.6044993	 |
| 	LATAM	 | 	Business Laptop	 | 	2021	 | 	1813.3458	 | 	1.34904	 | 	377.1759264	 | 	128.239815	 | 	93.61506493	 | 	55.14312044	 | 	1157.822833	 |
| 	LATAM	 | 	Business Laptop	 | 	2022	 | 	2782.7793	 | 	10.44978	 | 	550.9903014	 | 	333.3491323	 | 	136.6731443	 | 	350.016589	 | 	1401.300353	 |
| 	LATAM	 | 	Gaming Laptop	 | 	2019	 | 	1178.78	 | 	0.05588	 | 	278.19208	 | 	111.276832	 | 	50.0745744	 | 	57.86395264	 | 	681.316681	 |
| 	LATAM	 | 	Gaming Laptop	 | 	2020	 | 	1799.9345	 | 	0.15862	 | 	435.584149	 | 	150.2765314	 | 	132.2433476	 | 	94.67421479	 | 	986.9976372	 |
| 	LATAM	 | 	Gaming Laptop	 | 	2021	 | 	2417.7944	 | 	0.83688	 | 	469.0521136	 | 	197.0018877	 | 	133.9612836	 | 	161.5415479	 | 	1455.400687	 |
| 	LATAM	 | 	Gaming Laptop	 | 	2022	 | 	3091.977	 | 	8.40752	 | 	927.5931	 | 	389.589102	 | 	179.2109869	 | 	331.1507367	 | 	1256.025554	 |

Notes:
* Provided in .xlsx format
* This table contains data on the marketshare of various personal computer (PC) manufacturers (atliq, dale, innovo, pacer, bp). This marketshare data is available for each specific market subzone, PC product category, and fiscal year.
* The columns `sub_zone`, `category`, and `fy_desc` act as a **composite primary key**

<br>

</details>











## ETL (Extract Transform Load) using Power Query

<details>
  <summary><b>Import Data</b></summary>

The data tables from MySQL, .csv, and .xlsx were imported into **Power Query**:</br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/PowerQuery%20Initial%20Import.PNG)
</details>


<details>
  <summary><b>Additional Queries</b></summary>

<br>

**Add step to query: `fact_forecast_monthly`**

This step removes unnecessary redundant columns from `fact_forecast_monthly`
```
= Table.SelectColumns(fact_forecast_monthly, {"date", "product_code", "customer_code", "forecast_quantity"})
```
Sample records from query result:</br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/Forecast_Monthly%20remove%20redundant%20columns.PNG)

<br>

**Add step to query: `fact_sales_monthly`**

This step removes unnecessary redundant columns from `fact_sales_monthly`
```
= Table.SelectColumns(fact_sales_monthly,{"date", "product_code", "customer_code", "sold_quantity"})
```
Sample records from query result:</br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/Sales_Monthly%20remove%20redundant%20columns.PNG)

<br>

**Create new query: `Last_Sales_Month`**

This query generates a single date value representing the most recent month sales data is available in `fact_sales_monthly`
```
let
    LastSalesMonth = List.Max(fact_sales_monthly[date])
in
    LastSalesMonth
```
Query result:</br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/last%20sales%20month%20query%20result.PNG)

<br>

**Create new query: `Refresh Date`**

This query generates a single date value representing the most recent date the refresh button was pressed for this dashboard:
```
= DateTime.Date(DateTime.LocalNow())
```

<br>

**Create new query: `Combine Sales and Forecast`**

`Combine Sales and Forecast` needs to have:
1. Actual sales data from `fact_sales_monthly` for the time period up to and including the most recent month with sales data
2. Forecasted sales data from `fact_forecast_monthly` for the time period after the most recent month with sales data

`Combine Sales and Forecast` needs to combine the `fact_sales_monthly` query with the `fact_forecast_monthly` query based on the diagram below (similar to SQL Union):
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/Combined%20Sales%20and%20Forecast%20Diagram.PNG)

```
let
    // Filter the forecast table to only include records after the most recent month sales data was available
    #"FilterForecastTable" = Table.SelectRows(fact_forecast_monthly, each [date] > Last_Sales_Month),

    // Rename sold_quanity column in sales table to Qty
    #"Rename sold_quantity to Qty" = Table.RenameColumns(fact_sales_monthly, {{"sold_quantity", "Qty"}}),

    // Rename forecast_quantity column in forecast table to Qty
    #"Rename forecast_quantity to Qty" = Table.RenameColumns(fact_forecast_monthly, {{"forecast_quantity", "Qty"}}),

    // Union of Sales and Forecast tables
    UnionSalesForecast = Table.Combine({#"Rename sold_quantity to Qty", #"Rename forecast_quantity to Qty"})
in
    UnionSalesForecast
```
Sample records from query result:<br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/Combined%20Sales%20and%20Forecast.PNG)

<br>

**Create new query: `Fact_Actuals_Estimates`**

This query performs the following steps:
* Left join `Combine Sales and Forecast` with `gross_price`
* Left join `Combine Sales and Forecast` with `pre_invoice_deductions`
* Add calculated column for gross sales
* Add calculated column for net invoice sales
* Remove unnecessary columns, set appropriate datatype for columns

```
let


    // Add fiscal year column to act as a key field to match records in the left join
    #"Add fiscal year column" = 
        Table.AddColumn(
            #"Combine Sales and Forecast", 
            "fiscal_year", 
            each Date.Year(
                Date.AddMonths(
                    [date], 
                    4
                )
            )
        ),

    // Change datatype of fiscal_year column to text
    #"Changed fiscal_year column datatype" = 
        Table.TransformColumnTypes(
            #"Add fiscal year column", 
            {{"fiscal_year", type text}}
        ),

    // Perform a left join with gross_price table based on product_code and fiscal_year
    #"Left Join with gross_price" = 
        Table.NestedJoin(
            #"Changed fiscal_year column datatype", 
            {"product_code", "fiscal_year"}, 
            gross_price, 
            {"product_code", "fiscal_year"}, 
            "gross_price", 
            JoinKind.LeftOuter
        ),

    // Expand the gross_price column to include the actual gross price values
    #"Expanded gross_price" = 
        Table.ExpandTableColumn(
            #"Left Join with gross_price", 
            "gross_price",
            {"gross_price"},
            {"gross_price"}
        ),

    // Calculate gross sales amount (Qty * gross_price)
    #"Calculated Column for gross_sales_amount" = 
        Table.AddColumn(
            #"Expanded gross_price", 
            "gross_sales_amount", 
            each [Qty] * [gross_price]
        ),

    // Perform a left join with pre_invoice_deductions table based on customer_code and fiscal_year
    #"Left Join with pre_invoice_deductions" = 
        Table.NestedJoin(
            #"Calculated Column for gross_sales_amount", 
            {"customer_code", "fiscal_year"}, 
            pre_invoice_deductions, 
            {"customer_code", "fiscal_year"}, 
            "pre_invoice_deductions", 
            JoinKind.LeftOuter
        ),

    // Expand the pre_invoice_deductions column to get the discount percentage
    #"Expanded pre_invoice_deductions" = 
        Table.ExpandTableColumn(
            #"Left Join with pre_invoice_deductions", 
            "pre_invoice_deductions", 
            {"pre_invoice_discount_pct"}, 
            {"pre_invoice_discount_pct"}
        ),

    // Calculate net invoice sales (gross_sales_amount - pre-invoice discount amount)
    #"Calculated column for net_invoice_sales_amount" = 
        Table.AddColumn(
            #"Expanded pre_invoice_deductions", 
            "net_invoice_sales_amount", 
            each [gross_sales_amount] - [gross_sales_amount] * [pre_invoice_discount_pct]
        ),

    // Remove unnecessary columns
    #"Removed unnecessary redundant columns" = 
        Table.RemoveColumns(
            #"Calculated column for net_invoice_sales_amount", 
            {"fiscal_year", "gross_price", "pre_invoice_discount_pct"}
        ),

    // Set appropriate data types for the columns
    #"Set columns to appropriate datatypes" = 
        Table.TransformColumnTypes(
            #"Removed unnecessary redundant columns", 
            {
                {"gross_sales_amount", Currency.Type},
                {"net_invoice_sales_amount", Currency.Type}
            }
        )


in
    #"Set columns to appropriate datatypes"
```
Sample records from query result:</br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/Fact_Actuals_Estimates.PNG)

<br>

**Create new query: `dim_date`**

This query creates a date dimension table with three columns:
* `date` representing each calendar date. This is a primary key field.
* `month` representing each calendar month for each respective caldendar date
* `fiscal_year` representing AtliQ's fiscal year for each respective calendar date
```
let


    // Find minimum date from forecast table
    MinForecastDate = List.Min(fact_forecast_monthly[date]),

    // Find minimum date from sales table
    MinSalesDate = List.Min(fact_sales_monthly[date]),

    // Find the lower of MinForecastDate and MinSalesDate. This is the earliest date in dim_date table.
    StartDate = List.Min({MinForecastDate, MinSalesDate}),

    // Find maximum date from forecast table
    MaxForecastDate = List.Max(fact_forecast_monthly[date]),

    // Find maximum date from sales table
    MaxSalesDate = List.Max(fact_sales_monthly[date]),

    // Find the higher of MaxForecastDate and MaxSalesDate. This is the highest date in dim_date table.
    EndDate = List.Max({MaxForecastDate, MaxSalesDate}),

    // Create a list of dates from StartDate to EndDate and sort ascending
    DateList =
        List.Dates(
            StartDate,
            Duration.Days(EndDate - StartDate) + 1,
            #duration(1, 0, 0, 0)
        ),
    DateList_SortASC = List.Sort(DateList,Order.Ascending),

    // Convert list of dates to table and assign appropriate datatype to date column
    DateTable =
        Table.FromList(
            DateList_SortASC,
            Splitter.SplitByNothing(),
            {"date"}
        ),
    #"Changed data type of date column" = Table.TransformColumnTypes(DateTable,{{"date", type date}}),

    // Since data in forecast and sales tables are aggregated on a monthly level,
    // add a month column with values for the first day of each month
    #"Add month column" =
        Table.AddColumn(
            #"Changed data type of date column",
            "month",
            each Date.StartOfMonth([date]),
            type date
        ),

    // Add a text column for AtliQ's fiscal year by adding 4 months
    // to each calendar month and taking the year
    #"Add Fiscal Year column" =
        Table.AddColumn(
            #"Add month column",
            "fiscal_year",
            each Text.From(
                Date.Year(
                    Date.AddMonths([month], 4)
                )
            ),
            type text
        )


in
    #"Add Fiscal Year column"
```

Sample records from query result:<br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/dim_date%20query.PNG)

<br>

**Add steps to query: `Marketshare`**

Add two additional steps to the `marketshare` query:
1. Transform the table to make it more suitable for building data model and visuals later.
```
= Table.UnpivotOtherColumns(marketshare, {"sub_zone", "category", "fy_desc", "total_market_sales_$"}, "Manufacturer", "sales_$")
```
2. In the "Manufacturer" column, remove the text "sales_$" after the first "_" delimiter to make the manufacturer names clean.
```
= Table.TransformColumns(marketshare, {{"Manufacturer", each Text.BeforeDelimiter(_, "_"), type text}})
```
Sample records from query result:<br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/marketshare%20query.PNG)

<br>

</details>



<details>
  <summary><b>Data Cleaning</b></summary>

Data cleaning is a vital step to reduce the likelihood of errors and biases when business stakeholders use the final dashboard to inform the decision-making process.
Various data cleaning tasks were formed using Power Query (this list is not exhaustive):
* Identifying duplicate values and rectifying them with an appropriate method
* Investigating outliers in quantitative fields with business stakeholders and removing them if appropriate.
* Text fields: fixing spelling mistakes, removing extra white space
* Ensuring primary key fields contain unique values
* Ensuring composite primary key fields contain unique combinations of values
* Connecting with business stakeholders to determine an appropriate interpretation of null/blank values and rectifying them with an appropriate method if needed.

<br>

</details>

<details>
  <summary><b>Final Queries Loaded</b></summary>
The image below shows the final queries loaded from Power Query to Power BI. To improve query load time, queries not required to build the Power BI dashboard have their load disabled (queries in *italic* in the image below have their load disabled). Queries with their load disabled are either intermediate query steps or queries containing data that are already included in queries with their load enabled.<br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/final%20queries%20loaded.PNG)

</details>



## Data Modelling

<details>

  <summary><b>DAX Expressions to Create Tables</b></summary>

To help build the data model, three new dimension tables were created using DAX.

### `fiscal_year` table
```
fiscal_year = ALLNOBLANKROW(dim_date[fiscal_year])
```
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/dax%20fiscal%20year%20table.PNG)

### `sub_zone` table
```
// Unique market sub zones
sub_zone = ALLNOBLANKROW(dim_market[sub_zone])
```
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/subzone%20dax%20table.PNG)

### `category` table
```
// Unique product categories
category = ALLNOBLANKROW(dim_product[category])
```
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/category%20dax%20table.PNG)

</details>



<details>
  <summary><b>Building the Data Model</b></summary>

The image below shows the completed data model (snowflake schema) in Power BI Model View:<br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/data%20model%20dax.PNG)
</details>





<details>
  <summary><b>DAX Calculated Columns</b></summary>

To facilitate dashboard building, DAX expressions were used to create new columns in the tables `dim_date`, `dim_products`, and `Fact_Actuals_Estimates`

### Calculated Columns in `dim_date`
```
fiscal_quarter = 
SWITCH(
    TRUE(),
    MONTH(dim_date[date]) IN {9,10,11},
    "Q1",
    MONTH(dim_date[date]) IN {12,1,2},
    "Q2",
    MONTH(dim_date[date]) IN {3,4,5},
    "Q3",
    MONTH(dim_date[date]) IN {6,7,8},
    "Q4"
)
```
```
ytd_ytg = 

VAR current_fiscal_month = MONTH(DATE(YEAR(dim_date[date]), MONTH(dim_date[date]) + 4, 1))

VAR most_recent_calendar_month_with_sales = [Most_Recent_Month_With_Sales_Data]

VAR most_recent_fiscal_month_with_sales =
MONTH(
    DATE(
        YEAR(most_recent_calendar_month_with_sales),
        MONTH(most_recent_calendar_month_with_sales) + 4,
        1
    )
)

RETURN
IF(
    current_fiscal_month <= most_recent_fiscal_month_with_sales,
    "YTD",
    "YTG"
)
```

### Calculated Column in `dim_product`
```
product_and_variant = dim_product[product] & " [" & dim_product[variant] & "]"
```

### Calculated Columns in `Fact_Actuals_Estimates`
```
post_invoice_deduction_amount =
// Retrieve post invoice deduction percent for each row
VAR res = CALCULATE(
    MAX(post_invoice_deductions[discounts_pct]),
    RELATEDTABLE(post_invoice_deductions))

// Calculate post invoice deduction amount for each row
RETURN res * Fact_Actuals_Estimates[net_invoice_sales_amount]
```

```
post_invoice_other_deduction_amount =
// Retrieve other post invoice deduction percent for each row
VAR res = CALCULATE(
    MAX(post_invoice_deductions[other_deductions_pct]), 
    RELATEDTABLE(post_invoice_deductions))

// Calculate other post invoice deduction amount for each row
RETURN res * Fact_Actuals_Estimates[net_invoice_sales_amount]
```

```
// Calculate net sales (revenue) for each row
net_sales_amount = Fact_Actuals_Estimates[net_invoice_sales_amount] - Fact_Actuals_Estimates[post_invoice_deduction_amount] - Fact_Actuals_Estimates[post_invoice_other_deduction_amount]
```

```
manufacturing_cost =
// Retrieve manufacturing cost for each row
var res = CALCULATE(
    MAX(manufacturing_cost[manufacturing_cost]),
    RELATEDTABLE(manufacturing_cost))

// Calculate manufacturing cost for each row
RETURN res * Fact_Actuals_Estimates[Qty]
```

```
freight_cost =
// Retrieve freight cost for each row
var res = CALCULATE(
    MAX(freight_cost[freight_pct]),
    RELATEDTABLE(freight_cost))

// Calculate freight cost for each row
RETURN res * Fact_Actuals_Estimates[net_sales_amount]
```

```
// Retrieve other costs for each row
other_cost = 
var res = CALCULATE(MAX(freight_cost[other_cost_pct]), 
RELATEDTABLE(freight_cost))

// Calculate other costs for each row
RETURN res * Fact_Actuals_Estimates[net_sales_amount]
```

```
// Retrieve ads and promotions costs for each row
ads_promotion = 
var res = CALCULATE(
    MAX('operational_expenses'[ads_promotions_pct]),
    RELATEDTABLE('operational_expenses'))

// Calculate ads and promotions costs for each row
RETURN res * Fact_Actuals_Estimates[net_sales_amount]
```

```
// Retrieve other operational expense costs for each row
other_operational_expense = 
var res = CALCULATE(
    MAX('operational_expenses'[other_operational_expense_pct]),
    RELATEDTABLE('operational_expenses'))

// Calculate other operational expense costs for each row
RETURN res * Fact_Actuals_Estimates[net_sales_amount]
```
</details>













## DAX Measures

<details>
  <summary><b>Main KPIs</b></summary>

Gross Sales
```
GS_$ = SUM(FactActualsEstimates[gross_sales_amount])
```

Net Invoice Sales
```
NIS_$ = SUM(FactActualsEstimates[net_invoice_sales_amount])
```

Pre Invoice Deductions
```
Pre_Invoice_Deduction_$ = [GS_$] - [NIS_$]
```

Post Invoice Deductions
```
Post_Invoice_Deduction_Main_$ = SUM(FactActualsEstimates[post_invoice_deduction_amount])
```
```
Post_Invoice_Deduction_Other_$ = SUM(FactActualsEstimates[post_invoice_other_deduction_amount])
```
```
Post_Invoice_Deduction_Total_$ = [Post_Invoice_Deduction_Main_$] + [Post_Invoice_Deduction_Other_$]
```

Net Sales
```
NS_$ = SUM(FactActualsEstimates[net_sales_amount])
```

Cost of Goods Sold (COGS)
```
Manufacturing_Cost_$ = SUM(FactActualsEstimates[manufacturing_cost])
```
```
Freight_Cost_$ = SUM(FactActualsEstimates[freight_cost])
```
```
Other_Cost_$ = SUM(FactActualsEstimates[other_cost])
```
```
Total_COGS_$ = [Manufacturing_Cost_$] + [Freight_Cost_$] + [Other_Cost_$]
```

Gross Margin
```
GM_$ = [NS_$] - [Total_COGS_$]
```
```
GM_% = DIVIDE([GM_$], [NS_$], 0)
```
```
GM / Unit = DIVIDE([GM_$], SUM(FactActualsEstimates[Qty]), 0)
```

Operational Expenses
```
Ads_&_Promotions_$ = SUM(FactActualsEstimates[ads_promotion])
```
```
Other_Operational_Expense_$ = SUM(FactActualsEstimates[other_operational_expense])
```
```
Total_Operational_Expense_$ = [Ads_&_Promotions_$] + [Other_Operational_Expense_$]
```

Net Profit
```
NP_$ = [GM_$] - [Total_Operational_Expense_$]
```
```
NP_% = DIVIDE([NP_$], [NS_$], 0)
```
```
NP / Unit = DIVIDE([NP_$], SUM(FactActualsEstimates[Qty]), 0)
```

Marketshare
```
AtliQ_PC_Marketshare_% = 

VAR atliq_sales = 
CALCULATE(
    SUM(marketshare[sales_$]),
    marketshare[Manufacturer] = "atliq"
)

VAR total_market_sales = 
CALCULATE(
    SUM(marketshare[total_market_sales_$]),
    marketshare[Manufacturer] = "atliq"
)

RETURN
DIVIDE(
    atliq_sales,
    total_market_sales,
    0
)
```
```
PC_Marketshare_% = 
DIVIDE(
    SUM(marketshare[sales_$]),
    SUM(marketshare[total_market_sales_$]),
    0
)
```

Revenue Contribution %
```
RC_% = 
DIVIDE(
    [NS_$],
    CALCULATE(
        [NS_$],
        ALL(dim_market),
        ALL(dim_customer),
        ALL(dim_product)
    ),
    0
)
```

</details>






<details>
  <summary><b>Supply Chain KPIs</b></summary>

At AtliQ Technologies, supply chain metrics must be calculated for **each product on a montly level**. The screenshot below gives an example of how supply chain metrics are calculated for **one specific product** for a given fiscal year.
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/SupplyChain%20Example.PNG)


Last Sales Month
```
Most_Recent_Month_With_Sales_Data = MAX(LastSalesMonth[LastSalesMonth])
```

Sold Quantity
```
Sold_Quantity = 
CALCULATE(
    SUM(FactActualsEstimates[Qty]),
    FILTER(
        FactActualsEstimates,
        FactActualsEstimates[date] <= [Most_Recent_Month_With_Sales_Data]
    )
)
```

Forecasted Quantity
```
Forecasted_Quantity = 
CALCULATE(
    SUM(fact_forecast_monthly[forecast_quantity]),
    FILTER(
        fact_forecast_monthly,
        fact_forecast_monthly[date] <= [Most_Recent_Month_With_Sales_Data]
    )
)
```

Net Error and Inventory Risk
```
Net_Error = 
IF(
    ISBLANK([Sold_Quantity]) || ISBLANK([Forecasted_Quantity]),
    BLANK(),
    [Forecasted_Quantity] - [Sold_Quantity]
)
```
```
Inventory_Risk = 
SWITCH(
    TRUE(),
    ISBLANK([Sold_Quantity]) || ISBLANK([Forecasted_Quantity]),
    BLANK(),
    [Net_Error] > 0,
    "🔼 EI",
    [Net_Error] = 0,
    "PI",
    [Net_Error] < 0,
    "🚫 OOS"
)
```

Absolute Error
```
ABS_Error = 

VAR result = 
SUMX(
    DISTINCT(dim_date[month]),
    SUMX(
        DISTINCT(dim_product[product_code]),
        ABS([Net_Error])
    )
)

RETURN
IF(
    ISBLANK([Sold_Quantity]) || ISBLANK([Forecasted_Quantity]),
    BLANK(),
    result
)
```
```
ABS_Error_% = 

VAR result = 
DIVIDE(
    [ABS_Error],
    [Forecasted_Quantity],
    0
)

RETURN
IF(
    ISBLANK([Sold_Quantity]) || ISBLANK([Forecasted_Quantity]),
    BLANK(),
    result
)
```

Forecast Accuracy %
```
Forecast_Accuracy_% = 
IF(
    ISBLANK([ABS_Error_%]),
    BLANK(),
    1 - [ABS_Error_%]
)
```

</details>

## Dynamic Benchmark
<details>
  <summary><b>DAX Table</b></summary>

This dashboard enables users to compare certain KPIs against two types of benchmarks. A toggle switch allows users to switch between the following benchmark options:
1.	Year-over-Year (YoY) – Compares KPI values for the current time period to the same time period in the previous year.
2.	Target – Compares current KPI values to predefined business targets set by stakeholders.


To create this toggle switch (using slicer visual):<br>
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/BM%20toggle%20switch.PNG)<br>
where the user can choose which benchmark to show, a DAX calculated table `Benchmark_Switch_Table` was created:
```
Benchmark_Switch_Table = 
UNION(
    ROW("Primary_Key", 1, "Selection", "YoY"),
    ROW("Primary_Key", 2, "Selection", "Target")
)
```
![image alt](https://raw.githubusercontent.com/mike-li8/Power-BI-Business-Insights-360-II/refs/heads/main/Screenshots/BM%20Switch%20table.PNG)

</details>

<details>
  <summary><b>DAX Measures</b></summary>

**Filter Context Check**
Target benchmark data is only avaliable for the following KPIs: net sales, gross margin, and net profit. Since target data is only avaliable at the market level, the target benchmark should not be displayed when more granular filters such as products or customers are applied. To enforce this logic, the following DAX expression is used to check the filter context:
```
Customer_Product_FilterContext_Check = ISCROSSFILTERED(dim_product[product]) || ISFILTERED(dim_customer[customer])
```
When this measure returns true, it is not appropriate to display the target benchmark values related to net sales, gross margin, and net profit.

**Net Sales Benchmark Measures**
```
NS_$_SPLY = 
CALCULATE(
    [NS_$],
    SAMEPERIODLASTYEAR(dim_date[date])
)
```
```
NS_$_Target = 

VAR target = SUM(fact_targets[ns_target])

RETURN
IF(
    [Customer_Product_FilterContext_Check],
    BLANK(),
    target
)
```
```
NS_$_BM = 
SWITCH(
    TRUE(),
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 1, [NS_$_SPLY],
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 2, [NS_$_Target]
)
```
```
NS_$ Percentage Variance from BM = 

VAR result = DIVIDE([NS_$] - [NS_$_BM], ABS([NS_$_BM]), 0)

RETURN
IF(
    ISBLANK([NS_$]) || ISBLANK([NS_$_BM]),
    BLANK(),
    result
)
```

**Gross Margin Benchmark Measures**
```
GM_$_Target = 

VAR target = SUM(fact_targets[gm_target])

RETURN
IF(
    [Customer_Product_FilterContext_Check],
    BLANK(),
    target
)
```

**Gross Margin % Benchmark Measures**
```
GM_%_Target = 

VAR target = 
DIVIDE(
    SUM(fact_targets[gm_target]),
    SUM(fact_targets[ns_target]),
    0
)

RETURN
IF(
    [Customer_Product_FilterContext_Check],
    BLANK(),
    target
)
```
```
GM_%_SPLY = 
CALCULATE(
    [GM_%],
    SAMEPERIODLASTYEAR(dim_date[date])
)
```
```
GM_%_BM = 
SWITCH(
    TRUE(),
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 1, [GM_%_SPLY],
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 2, [GM_%_Target]
)
```
```
GM_% Variance from BM = 

VAR result = [GM_%] - [GM_%_BM]

RETURN
IF(
    ISBLANK([GM_%]) || ISBLANK([GM_%_BM]),
    BLANK(),
    result
)
```
```
GM_% Percentage Variance from BM = 

VAR result = DIVIDE([GM_% Variance from BM], ABS([GM_%_BM]), 0)

RETURN
IF(
    ISBLANK([GM_% Variance from BM]) || ISBLANK([GM_%_BM]),
    BLANK(),
    result
)
```

**Net Profit Benchmark Measures**
```
NP_$_Target = 

VAR target = SUM(fact_targets[np_target])

RETURN
IF(
    [Customer_Product_FilterContext_Check],
    BLANK(),
    target
)
```


**Net Profit % Benchmark Measures**
```
NP_%_SPLY = 
CALCULATE(
    [NP_%],
    SAMEPERIODLASTYEAR(dim_date[date])
)
```
```
NP_%_Target = 

VAR target = 
DIVIDE(
    SUM(fact_targets[np_target]),
    SUM(fact_targets[ns_target]),
    0
)

RETURN
IF(
    [Customer_Product_FilterContext_Check],
    BLANK(),
    target
)
```
```
NP_%_BM = 
SWITCH(
    TRUE(),
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 1, [NP_%_SPLY],
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 2, [NP_%_Target]
)
```
```
NP_% Variance from BM = 

VAR result = [NP_%] - [NP_%_BM]

RETURN
IF(
    ISBLANK([NP_%]) || ISBLANK([NP_%_BM]),
    BLANK(),
    result
)
```
```
NP_% Percentage Variance from BM = 

VAR result = DIVIDE([NP_% Variance from BM], ABS([NP_%_BM]), 0)

RETURN
IF(
    ISBLANK([NP_% Variance from BM]) || ISBLANK([NP_%_BM]),
    BLANK(),
    result
)
```

**Supply Chain Benchmark Measures**
YoY is the only benchmark available and/or applicable to supply chain KPIs.
```
Net_Error_SPLY = 
CALCULATE(
    [Net_Error],
    SAMEPERIODLASTYEAR(dim_date[date])
)
```
```
Net_Error_BM = 
SWITCH(
    TRUE(),
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 1, [Net_Error_SPLY],
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 2, BLANK()
)
```
```
ABS_Error_SPLY = 
CALCULATE(
    [ABS_Error],
    SAMEPERIODLASTYEAR(dim_date[date])
)
```
```
ABS_Error_BM = 

SWITCH(
    TRUE(),
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 1, [ABS_Error_SPLY],
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 2, BLANK()
)
```
```
ABS_Error_Percentage_Variance_from_BM = 

VAR result = DIVIDE([ABS_Error] - [ABS_Error_BM], ABS([ABS_Error_BM]), 0)

RETURN
IF(
    ISBLANK([ABS_Error]) || ISBLANK([ABS_Error_BM]),
    BLANK(),
    result
)
```
```
Forecast_Accuracy_%_SPLY = 
CALCULATE(
    [Forecast_Accuracy_%],
    SAMEPERIODLASTYEAR(dim_date[date])
)
```
```
Forecast_Accuracy_%_BM = 
SWITCH(
    TRUE(),
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 1, [Forecast_Accuracy_%_SPLY],
    SELECTEDVALUE('Benchmark_Switch_Table'[Primary_Key]) = 2, BLANK()
)
```
```
Forecast_Accuracy_%_Percentage_Variance_from_BM = 

VAR result = DIVIDE([Forecast_Accuracy_%] - [Forecast_Accuracy_%_BM], ABS([Forecast_Accuracy_%_BM]), 0)

RETURN
IF(
    ISBLANK([Forecast_Accuracy_%]) || ISBLANK([Forecast_Accuracy_%_BM]),
    BLANK(),
    result
)
```

</details>
