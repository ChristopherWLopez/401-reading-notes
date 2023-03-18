# class 31 reading

## What can React Context provide your app?

Context can make it easier to pass data (from parent to child) easily, where as using props would be more cumbersome especially when that data is UI Themes and Locale Data. With Context we are able to share value

## Why might we use Context?

We are able to share "global" data between components.

## Why should we use it sparingly?

Although it can be make things easy to pass certain value's down into nested components, its trade off is that it makes component reuse more difficult.

## Consume content from (at least) two of the Awesome React Context links. Share your take-away from each

## Takeaway 1

Using context allows you to send props/ state/ methods to non direct children of the component we are working on. This saves is from prop drilling. By using provider we are able to place the data that we want to make accessible and than within any child component we want to have access to that data we creat a consumer.

## Takeaway 2

This is a less relavant one but I liked how in the first video he used dot notation and specific properties value and assigned it to a variable. This was used to get a cleanely neamed variable from the `MyContext.Provider` and the `MyContext.Consumer`
