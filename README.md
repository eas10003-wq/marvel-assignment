# Marvel Universe Characters CSV — Three Data Questions

## Why I Chose This Dataset
I chose the Marvel Universe Characters dataset because superheroes and villains are fun and interesting. Each row represents a character, and the columns describe attributes like Role, Power Level, and Character name. It’s easy to explore simple questions, while still having clear limitations (e.g., Power Level is categorical, not a numeric measure of strength).


## Three Data Questions

# Question 1: How many characters are Heroes, Villains, or Other?
# role_counts = {}
# for row in marvel:
#     r = row["Role"]
#     if r in role_counts:
#         role_counts[r] += 1
#     else:
#         role_counts[r] = 1
# print(role_counts)
# output (example): Hero 50, Villain 20, Other 5

Why the data structure supports this question:
Each row is one character, and the Role column is categorical. Counting the frequency of each category is straightforward.

# Question 2: How many characters have Low, Medium, or High Power Levels?
# power_counts = {}
# for row in marvel:
#     p = row["Power Level"]
#     if p in power_counts:
#         power_counts[p] += 1
#     else:
#         power_counts[p] = 1
# print(power_counts)
# output (example): Low 40, Medium 25, High 10

Why the data structure supports this question:
The Power Level column is categorical, so it’s easy to count characters by each level. Each row is one character.

# Question 3: What are the first 10 characters with their Role and Power Level?
# for row in marvel[:10]:
#     print(row["Character"], row["Role"], row["Power Level"])
# output (example):
# iron man Hero Low
# captain america Hero Low
# thor Hero Medium
# ...

Why the data structure supports this question:
The dataset has columns Character, Role, and Power Level. Selecting the first 10 rows and printing them is simple and shows a small sample of the data.

---

## What the Data Cannot Answer
I wish I could answer which characters are the most popular among fans or appear in the most comics. This dataset only includes things like Role, Power Level, and Character name. It does not contain popularity data. This would mean it would assume popularity or strength based on this dataset which would be misleading.
