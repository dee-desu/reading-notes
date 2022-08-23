# States and props 
## Reading

**1- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

the render which is in the render phase.

**2- What is the very first thing to happen in the lifecycle of React?**

The Mounting phase in this order: Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount.

**3- Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates.**

Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount.

**4- What does componentDidMount do?**

This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. Ex: using the componentDidMount() to connect to the twitter API and get tweets when the component is rendered.

---
## Videos

**1- What types of things can you pass in the props?**

Components; such as the counter component it also enables you to pass values from one component to another.

**2- What is the big difference between props and state?**

is that in props you pass into a component and state is handled inside of that component and props are handled outside the component.

**3- When do we re-render our application?**

When you change the state inside of your application its going to re-render that sections of your application.

**4- What are some examples of things that we could store in state?**

We need state to put a counter to the app so that it keep updating, we also use it inside a form for elements like checkboxes select boxes.

