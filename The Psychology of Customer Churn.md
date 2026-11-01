We often say that data is information.

But raw data is not information. Not yet.

It is more like an unfinished conversation: scattered facts, missing answers, strange entries, and patterns waiting to be noticed. Before data can tell us anything useful, someone has to question it, clean it, and listen carefully.

That is where the work of a data analyst begins.

When I received a telecom customer churn dataset containing 7,043 customers, I entered it with one question:

**Why are customers leaving?**

People rarely leave without a reason.

They leave jobs when they feel undervalued. They leave relationships when trust disappears. They stop visiting businesses when they feel ignored. In the same way, customers cancel subscriptions when the service no longer feels worth staying for.

I began treating the dataset almost like a psychologist would approach a patient—not to judge it quickly, but to understand what was happening beneath the surface.

## First, I Had to Understand the Silence

Before analysing customer behaviour, I had to clean the data.

Missing values are often treated as empty spaces, but an empty cell does not always mean that information is unknown. Sometimes the blank itself has meaning.

For example, missing values in the `offer` column represented customers who had not received an offer. I replaced those blanks with **“No Offer.”**

The missing values in `churn_reason` told a different story. Customers who had stayed with the company naturally had no reason for leaving, so I labelled those values **“Not Applicable.”**

The same blank space meant two different things in two different columns.

That was an important lesson:

**Data cleaning is not only about writing code. It is about understanding context.**

I also found 120 negative values in the `monthly_charge` column. Since a telecom bill cannot realistically be negative, those values were clearly incorrect.

Deleting all 120 rows would have removed other useful customer information. Instead, I converted the invalid charges into missing values and replaced them with the median monthly charge.

Only after removing these inconsistencies was the dataset ready to speak.

## The First Warning Sign

Out of 7,043 customers, 1,869 had churned.

That gave the company a churn rate of approximately **26.54%**.

In simple words, more than one out of every four customers had left.

This was not a small leak. It was a warning signal.

The company was also losing approximately \*\*$\*\*139342.15 **every month** in recurring revenue from churned customers.

But money was only the visible loss.

Behind every cancelled subscription was a decision.

The deeper question was not:

**How many customers left?**

It was:

**What made leaving more attractive than staying?**

## Competitors Were Winning

The strongest pattern appeared in the churn reasons.

- 313 customers left because a competitor had better devices.
- 311 received a better offer elsewhere.
- 117 were offered more data.
- 100 were offered higher download speeds.

Together, these competitor-related reasons accounted for around **45% of all churned customers**.

Nearly half of the customers who left had not stopped needing telecom services. They had simply moved to another provider.

The demand was still there.

The customer was still willing to pay.

But another company appeared to offer more value.

This means the company was not only losing customers. It was losing a competition involving devices, pricing, speed, data, and offers.

Customers compare, even when companies do not.

To reduce this kind of churn, the company must regularly study what competitors are offering and ask:

- Are our plans still attractive?
- Are our devices competitive?
- Are customers receiving enough data?
- Does the service justify its price?
- Are high-value customers receiving suitable retention offers?

## When Communication Becomes a Business Problem

One of the most striking findings was related to customer service.

Around 220 customers left because of the attitude of a support person. Another 94 customers were dissatisfied with the attitude of the service provider.

Others mentioned poor support knowledge, service dissatisfaction, and limited self-service options.

These customers did not always leave because the entire telecom service had failed.

Many left because the conversation had failed.

A company may invest in infrastructure, advertising, software, fibre networks, and new products. Yet one careless interaction can damage the trust built through all those investments.

Customers may forget the exact words spoken during a support call, but they often remember how the conversation made them feel.

Were they heard?

Were they respected?

Was their problem taken seriously?

Or were they treated like another complaint number?

Customer support is not separate from the product. It is part of the product.

Training support teams to communicate with patience, empathy, and clarity could prevent a meaningful share of churn. Faster complaint resolution, stronger technical knowledge, and better self-service tools could also make customers feel supported rather than ignored.

Sometimes retaining a customer does not require advanced technology.

Sometimes it requires a better conversation.

## Why Were Month-to-Month Customers Leaving?

Another strong pattern appeared in contract type.

Customers with month-to-month contracts were more likely to churn, while customers with one-year and two-year contracts were more likely to stay.

The reason may be simple: month-to-month customers have greater freedom.

They can leave quickly when prices increase, service quality falls, or a competitor makes a better offer.

Long-term customers may stay because they receive discounts, enjoy predictable pricing, or have already committed to the company.

But this does not mean long contracts automatically create satisfaction.

A contract may delay churn, but it cannot create loyalty by itself.

The company should not make leaving difficult. It should make staying valuable.

Month-to-month customers could be encouraged to choose longer plans through:

- Discounted annual packages
- Loyalty rewards
- Free upgrades
- Extra data
- Device benefits
- Price protection
- Flexible cancellation terms

The goal should not be to lock the customer in.

The goal should be to give them a reason to remain.

## The Fibre-Optic Puzzle

One finding surprised me: fibre-optic customers appeared to churn more frequently.

At first, this seemed strange. Fibre optic is usually presented as a premium service with higher speed and better performance.

So why were fibre customers leaving?

The answer may not be the technology itself.

Fibre customers may pay higher monthly charges and therefore expect premium performance. Even a small interruption may feel serious when the customer is paying more.

They may also be targeted by competitors offering better speeds, lower prices, free installation, or attractive introductory plans.

Another possibility is that many fibre users also have month-to-month contracts or received no promotional offer.

This is why a pattern should not be treated as a final answer.

It should be treated as a clue.

To understand the real reason, fibre customers should be compared across:

- Monthly charges
- Contract type
- Tenure
- Offers received
- Payment method
- Network complaints
- Customer support experience
- Churn reasons

Good analysis does not stop after finding an unusual pattern.

It asks what may be hiding behind it.

## Customers Without Offers Were Leaving More

Customers who had not received any offer also appeared more likely to churn.

This suggests that promotional offers may influence retention.

However, giving the same discount to every customer would not be an intelligent solution.

Different customers leave for different reasons.

A customer unhappy with price may appreciate a discount.

A customer frustrated by poor network performance may prefer a technical upgrade.

A customer considering a competitor may value more data, higher speed, or a better device.

A customer upset with support may simply want their complaint resolved properly.

The offer should match the problem.

The company could target personalised offers toward customers who are more likely to leave, such as:

- Month-to-month subscribers
- Customers with low tenure
- High-paying fibre users
- Customers who recently contacted support
- Customers with repeated complaints
- Customers who have never received an offer

A general offer says, “Here is a discount.”

A personalised offer says, “We understand what you need.”

## The Customers Who Left Without Explaining

Around 130 customers had **“Don’t know”** recorded as their churn reason.

This may appear to be a small category, but it represents a major blind spot.

When a customer leaves without giving a clear reason, the company loses more than revenue. It loses the opportunity to learn.

Short exit surveys, cancellation forms, follow-up calls, and better reason categories could help the company understand future departures.

Every customer who leaves carries information.

The company must create a respectful way to collect it.

## What the Company Can Learn

The analysis points toward a few clear actions.

The company should improve its competitive position by reviewing devices, plans, data allowances, speeds, and pricing.

It should treat communication as a business priority and provide better training to support teams.

It should create meaningful incentives for month-to-month customers to move toward longer plans.

It should investigate fibre-optic churn more carefully instead of assuming that fibre technology itself is the problem.

It should use personalised retention offers rather than giving every customer the same promotion.

Finally, it should improve the way churn reasons are collected.

The lesson is simple:

**Do not only count the customers who leave. Listen to what their leaving is trying to say.**

## Final Reflection

This project helped me understand that churn is not merely a percentage.

Behind every churned record was a customer who made a decision.

Some found better services elsewhere.

Some felt the price was too high.

Some experienced unreliable networks.

Some were disappointed with the product.

And some simply did not feel respected during an interaction with customer support.

The churn rate of 26.54% was not only a business metric.

It was the collective voice of customer dissatisfaction.

A psychologist listens to words, silence, emotions, and patterns.

A data analyst listens to values, missing entries, categories, and relationships.

Both look beneath the surface.

Both question the obvious answer.

And both are ultimately trying to understand the same thing:

**What is the story behind the behaviour, and what can we learn from it?**

## The Story Behind the Story

Every insight in this article began with a line of code, a question, and the patience to look beneath the obvious answer. You can explore the complete data-cleaning process, analysis, visualizations, and code in my GitHub repository.

**Explore the complete project:** [Telecom Customer Churn Analysis](https://github.com/meemp21-code/Telecom_churn)
