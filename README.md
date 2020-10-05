# NU Technology Nodejs Coding Challenge

Welcome to the NU Technology Nodejs coding challenge! Please read the following instructions carefully.

**Your goal is to set up an Nodejs api endpoint which returns the product listing JSON response.**

# Contents

-   [Business need](#business-need)
-   [Use cases](#use-cases)
-   [Sample Data](#sample-data)
-   [Evaluation criteria](#evaluation-criteria)
    -   [Technology requirements](#technology-requirements)
    -   [Code requirements](Criteria.md#must-have)
-   [How to submit](#how-to-submit)
-   [Time limit](#time-limit)

# Business need

The main goal is for the api is to return the product listing mock data in JSON response.


# Use cases

- Should be able to access the api enpoint via {server host}**/product-listing**
  - Should return the response in JSON format
  - Should retun the status code as 200 OK
- Any other request except **/product-listing** should be routed to 404
  - Should return response body as null
  - Should retun the status code as 404

Note:- Configure the api server to run on port 9000.

# Sample Data
- Use the below sample JSON
```{
  "facets": [
    {
      "facetId": "price_f",
      "name": "Price",
      "position": 2,
      "values": {
            "counts": [
              "0",
              4,
              "300",
              4,
              "400",
              2
            ],
            "gap": 100,
            "start": 0,
            "end": 2000
          }
    },
    {
      "facetId": "color_f",
      "name": "Color",
      "position": 3,
      "values": ["Black", "Blue", "Pink", "Green", "Red"]
    },
    {
      "facetId": "gender_f",
      "name": "Gender",
      "position": 1,
      "values": ["men", "women"]
    }
  ],
  "catalog": [
    {
      "id": 1,
      "imageURL": "http://placehold.it/150/1b21a0/ffffff",
      "name": "product A",
      "type": "",
      "price": 250,
      "currency": "$",
      "color": "Black",
      "gender": "men"
    },
    {
      "id": 2,
      "imageURL": "http://placehold.it/150/bc4125/ffffff",
      "name": "product B",
      "type": "",
      "price": 350,
      "currency": "$",
      "color": "Blue",
      "gender": "women"
    },
    {
      "id": 3,
      "imageURL": "http://placehold.it/150/5abc25/ffffff",
      "name": "product C",
      "type": "",
      "price": 150,
      "currency": "$",
      "color": "Pink",
      "gender": "men"
    }
  ]
}
```

# Evaluation criteria

## Technology requirements

**Nodejs** with **Express** are the mandatory requirements. Apart from this, you can use any libraries. ES6 and build processors are highly encouraged.

## Code requirements

The full criteria for evaluating the coding challenge can be found [here](./Criteria.md).

# How to submit

- If you are using https://codesandbox.io/
  - In the menu section go to File -> Export to ZIP
  - Email the zipped file to your point of contact.

- If you are developing on your machine
  - Clone this repository.
  - Complete your project as described above within your local repository.
  - Ensure everything you want to commit is committed before you bundle.
  - Create a git bundle: `git bundle create your_name.bundle --all`
  - Email the bundle file to your point of contact.

**In order to be fair to all candidates, please refrain from sharing your solution on public repository hosting services such as GitHub and Bitbucket.**

# Time limit

There is no hard time limit for this coding challenge. However, we believe that 1-2 hours is sufficient for the must-have parts of the application. While we appreciate all the effort put into the challenge, we also do not want to take up too much of your time. Our advice is to focus on making sure [that the application works properly and has some tests](Criteria.md#must-have) before moving on to secondary objectives.

Good luck,
The NU Technology Team
