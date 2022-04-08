# My CCAH Assessment Answers

**Question 1:** You are attempting to make several visual/layout changes to a web page. If you only have one chance to place your code, how do you ensure/test that it’s correct? 

**Answer:** Most of the time, when developing you will have access to a development server which provides a runtime environment. This allows you to see how the page looks running in your browser while you make changes to it. If you do not have this, it is still possible to open any HTML file in your browser, which allows you to see  (roughly) how your code will look when loaded by a user’s browser. 

While you are viewing the document in your browser, you can use something like Chrome Dev Tools to preview how things will look on different types of screens. I also like using Google Chrome's Lighthouse feature to do an audit of my code that can catch when you have unnecessary/unused code and give you suggestions for improving accessibility. 

Finally, you can use unit testing tools like Jest to make sure your functions and components are working as intended.   

<br>

**Question 2:** Imagine you have a web page with a form for users to fill out and submit. Can you think of a way that the page can save the user's progress if they leave (close web page or navigate away) and come back later using front end code only?

**Answer:** It is possible to set up a form to save a user’s input to local storage, which would save the input data. If you do this, you would also need to retrieve any input from local storage to repopulate the form fields.

**My Code Snippet For Question 3:**

``` 

function getQueryValue(key) {
    let params = new URLSearchParams(document.location.search)
    let keyValue = params.get(key)
    return keyValue
  }

  if (getQueryValue("content") == "returning") {
      document.querySelector('p').innerHTML = "Welcome Back!"
    }

```

**[Link to my files for Question 4](https://github.com/nick-zanetti/ccah-assess)** (or navigate to the base of this repo) 
