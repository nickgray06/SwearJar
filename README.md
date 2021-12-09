# README

# Better Budgeting Sytems
-> All your finances in one place! <-


## Table of Contents
- [General Info](#general-info)
- [Technologies](#technologies)
- [Setup](#setup)
- [Features](#features)
- [Code Example](#code-example)
- [Status](#status)
- [Inspiration](#inspiration)
- [Contact](#contact)


## General Info
Swear Jar allows you to take make amends of poor language by donating to charity!


# Technologies 
- Ruby
- Javascript
- RubyERB
- HTML
- CSS
- Stripe API


## Setup 
To run Better Budgeting Sytems!, fork and clone this GitHub repository. Then run:

cd into backend

run bundler

yarn watch

cd into frontend

npm install

npm start



## Code Example

```react
const [transactions, setTransactions] = useState([]);

  useEffect(() => {
    if (!props.accessToken) {
      return;
    }
    const accessToken = props.accessToken;
    async function iWantTransactions() {
      let res = await axios.post("http://localhost:8080/transactions", {
        accessToken: accessToken,
      });
      console.log(res);
      let transactions = res.data.transactions;
      setTransactions(transactions);
      console.log(transactions);
    }
    iWantTransactions();
  }, [props.accessToken]);
```

## Features
- Links to Stripe API to connect payment
- Can donate to selected charities
- Remembers previous users accounts


## Status
This project is currently finished. I may introduce new features or refactor existing code going forward.


## Inspiration
I built Swear Jar as my Mod 3 project. 


## Contact
Swear Jar was created by [Nick Gray](https://www.linkedin.com/in/nick-gray-06/)

Feel free to reach out!
