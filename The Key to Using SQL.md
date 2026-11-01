First of all, let's understand what **keys** are. 🗝️

**Keys** are attributes, or combinations of attributes, that uniquely identify each record (row) in a table and help establish relationships between different tables.

There are **7 types of keys in a database** that we will discuss here.

Let's create a simple table and understand them one by one.

### Student Table ⬇️

| Roll No | Name | Branch | Email |
| --- | --- | --- | --- |
| 101 | Rohit Sharma | ECE | [rohits@college.com](mailto:rohits@college.com) |
| 102 | Neha | EEE | [nehas@college.com](mailto:nehas@college.com) |
| 103 | Rohit Mehra | ECE | [mehra@college.com](mailto:mehra@college.com) |

Here, **Roll No** and **Email** are unique, so they can become keys.

Two students cannot have the same Roll No or Email, but they can have the same Name or belong to the same Branch.

For example, if I look into the records and call out **Roll No 102**, I can immediately pull out Neha's record.

But if I make **Name** the key and simply call out "Rohit," I will be confused.

Which Rohit am I talking about?

Rohit Sharma or Rohit Mehra?

Now take a look at your 10th marksheet. Your roll number was assigned to uniquely identify you during that examination, while things like your email ID may change over time.

Since the basic concept of keys is clear, let's move on to the different types of keys.

### 1\. Super Key: Any group of columns that can pick out one student

In our table, **Roll No** can work as a Super Key.

But these combinations can also work:

```plaintext
Roll No + Name
Roll No + Branch
Roll No + Email
Roll No + Branch + Email
Roll No + Branch + Name
Roll No + Branch + Name + Email
```

all combinations work (even though they are extra).

Any combination that can uniquely find a student is a **super key.**

### 2\. Candidate Key: The smallest group that can pick out one student

In our table **Roll no** and **Email** can be candidate keys, because they are the shortest description to find out a student.

### 3\. Primary Key: The one Candidate Key the teacher picks as the official ID

In our table, we can make **Roll No** our Primary Key.

But why choose Roll No instead of Email?

Because there are some important rules for choosing a Primary Key.

**Rules:**

- **No duplicate values:** No two students can share the same value.
- **Cannot be NULL:** Every student must have a value for the Primary Key.

There may be situations where a student does not have an email ID, or their email ID changes, but every student in the school/college database can be assigned a unique Roll No.

That's why Roll No is a better choice for the Primary Key.

Think of it like your Aadhaar number — it is used as a unique identifier for you.

### 4\. Alternate Key: The Candidate Keys we *didn't* pick as the Primary Key

Remember, we had two Candidate Keys:

**Roll No** and **Email**

We selected **Roll No** as our Primary Key.

So, **Email** becomes the Alternate Key.

It is still capable of uniquely identifying a student, but it wasn't selected as the official Primary Key.

Think of it as the **backup ID**.

### 5\. Foreign Key: A column that points to another table's Primary Key

Now imagine we have another table called **Branches**.

### Branches Table

| Branch ID | Branch Name |
| --- | --- |
| 1 | EEE |
| 2 | ECE |

Instead of storing the Branch Name again and again in our Student Table, we can store the **Branch ID**.

Our Student Table could look like this:

| Roll No | Name | Branch ID | Email |
| --- | --- | --- | --- |
| 101 | Rohit Sharma | 2 | [rohits@college.com](mailto:rohits@college.com) |
| 102 | Neha | 1 | [nehas@college.com](mailto:nehas@college.com) |
| 103 | Rohit Mehra | 2 | [mehra@college.com](mailto:mehra@college.com) |

Here, **Branch ID** in the Student Table points to **Branch ID** in the Branches Table.

So, **Branch ID** in the Student Table becomes a **Foreign Key**.

For example:

**Branch ID = 1 → EEE**

**Branch ID = 2 → ECE**

It's like a **post-it note** on your locker that says, *"I belong to Room 1."*

The Foreign Key connects one table to another.

### 6\. Composite Key: Two or more columns together make a unique ID

Sometimes, one column alone is not enough to uniquely identify a record.

In that case, we can combine two or more columns.

That combination is called a **Composite Key**.

For example, imagine we have a table where neither Name nor Email alone is sufficient for our requirement, but their combination is unique.

```plaintext
Name + Email
```

Together, they can identify one student.

That's a Composite Key.

Think of it like saying: *T****he girl in the blue dress***\*.\* **Girl** alone isn't enough. **Blue dress** alone may not be enough.

But when you combine both clues, it becomes easier to identify the person.

### 7\. Surrogate Key: A key we create ourselves

Sometimes, the existing columns are not suitable for becoming a Primary Key.

Let's look at this table:

| Name | Branch | CGPA |
| --- | --- | --- |
| Rahul | CSE | 8.5 |
| Rahul | ECE | 8.5 |
| Rishi | CSE | 9.5 |

Here, Name is not unique.

Branch is not unique.

CGPA is also not unique.

Instead of depending on these values, we can add a new column ourselves.

| ID | Name | Branch | CGPA |
| --- | --- | --- | --- |
| 1 | Rahul | CSE | 8.5 |
| 2 | Rahul | ECE | 8.5 |
| 3 | Rishi | CSE | 9.5 |

Now we have an **ID** that uniquely identifies every record.

This ID is called a **Surrogate Key**.

A Surrogate Key doesn't necessarily have any real-world meaning. It is mainly created to uniquely identify records in the database.

You will often see columns like:

```plaintext
student_id
customer_id
order_id
product_id
```

These are commonly used as Surrogate Keys.

## Quick Cheat Sheet

| Key | One-line explanation |
| --- | --- |
| **Super Key** | Any "description" that uniquely finds one student, even if it contains extra information |
| **Candidate Key** | The shortest possible description that uniquely finds one student |
| **Primary Key** | The official Candidate Key chosen to identify each record |
| **Alternate Key** | A Candidate Key that wasn't chosen as the Primary Key |
| **Foreign Key** | A column that points to a key in another table |
| **Composite Key** | Two or more columns that work together to uniquely identify a record |
| **Surrogate Key** | An artificial ID created to uniquely identify records |

Now, take a dataset for and try to find out the keys by yourself.

Happy learning😊
