---
layout: post
title: Subscription Management app
subtitle: Mobile app created as part of my Final Year Project
tags: [Java, Project]
comments: true
---

This post contains information regarding the Subscription Management app that I created as my final year project. It also provides some code snippets to show its technical aspects.  
This app allows the users to:  
* Add subscriptions
* View the added subscriptions and their details
* Edit the subscriptions
* View the total amount they spend on subscriptions:
  * Monthly
  * Every 3 months
  * Every 6 months
  * Annually   

## Here is a secondary heading

Here's a useless table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |


## Home Screen

![image](/assets/img/New Home Screen (Green).PNG){: .mx-auto.d-block :}

## Add a subscription screen

![image](/assets/img/new-add-sub.png){: .mx-auto.d-block :}

## Subscription information screen

![image](/assets/img/New Sub Info.PNG){: .mx-auto.d-block :}

## Settings screen

![image](/assets/img/Settings.PNG){: .mx-auto.d-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

### Here is part of my code that displays the subscriptions and calculates the monthly total:

```java
for (DataSnapshot childSnapshot : dataSnapshot.getChildren()) {
      String name = childSnapshot.child("name").getValue(String.class);
      String frequency = childSnapshot.child("frequency").getValue(String.class);

      try{
          //format price number so that it is in the Double form
          Double amountTemp = Double.valueOf(formattedTotal.format(Double.valueOf
                  (childSnapshot.child("price").getValue(String.class))));

          //Calculate the monthly cost of each subscription
          if (frequency.equals("Yearly")){
              amountTemp = amountTemp/12;
          }
          else if (frequency.equals("Every 6 months")){
              amountTemp = amountTemp/6;
          }
          else if (frequency.equals("Every 3 months")){
              amountTemp = amountTemp/3;
          }
          total = total + amountTemp; // calculate the monthly total of the subscriptions
          subscriptions.add(name);
      }
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.
