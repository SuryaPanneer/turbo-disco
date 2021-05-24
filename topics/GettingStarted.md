---
course: TWT
date: May 23, 2021
author: Surya
layout: template
link: Intro
---

This view returns information about customers of the organization and person types in Oracle Fusion Receivables. This information is accessible through Receivables > Billing work area > Manage Customers. A record is returned for each customer identifier.

<p.note>Note: This view returns information only about customers while the Manage Customers page may display information about all parties, such as suppliers and customer contacts.</p>

<h1>My period of stay in the last 5 years is as follows:</h1>

{% for item in site.data.common %}
- {{item.period}}, {{item.place}}
{% endfor %}

**Description**

This view provides the following details:
- Customer information, such as the name, number, language, Data Universal Number System (DUNS) number, category, address, and number of employees
- Person- type customer information, such as the name, date of birth, and primary phone number; organization-type customer information, such as the chief executive officer (CEO) name, potential revenue of the customer in the current year and next year, Standard Industrial Classification (SIC) code, line of business, mission statement, home country, and legal status. The Disadvantaged_8A_Flag column indicates whether the customer is eligible for the 8(a) program. The Internal_Organization_Flag column indicates whether the customer organization is an internal organization. The Customer_Type column indicates whether the customer type is "Organization" or "Person". The Small_Business_Flag column indicates whether the customer organization is certified as a small business organization. The Dun_Bradstreet_Rating column indicates the Dun and Bradstreet rating of the customer.

**Performance**

For optimal performance, filter the records by the Customer_Type column.

This page was created as part of the {{page.course}} on {{page.date}} by {{page.author}}.

Read the [Stone Soup]({{page.link}}) story.
