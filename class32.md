# What are custom hooks?

Custom Hooks are a convention that naturally follows from the design of Hooks, rather than a React feature.

Custom Hooks offer the flexibility of sharing logic that wasn’t possible in React components before. You can write custom Hooks that cover a wide range of use cases like form handling, animation, declarative subscriptions, timers, and probably many more we haven’t considered. What’s more, you can build Hooks that are just as easy to use as React’s built-in features.

## useClippy

A hook for copying data to the clipboard and retrieving/pasting it using Ctrl-C/Command-C and Ctrl-V/Command-V.

we destructure the useClippy to clipboard and setClipboard. clipboard is the data in the clipboard and setClipboard sets the data in the clipboard.

## useBrowserContextCommunication

useBrowserContextCommunication uses the Broadcast Channel API to deliver an easy solution for communication between different browser contexts (tabs, iframes, windows).

it returns an array that has two items. The first is a communication state. This state contains lastMessage and messages which is an array of the messages that were sent from other tabs/windows to the current one. The second item is a function used to send messages to the other context.

## useScript

useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically.

``` import useScript from "react-script-hook"

function Component() {
    const [ loading, error ] = useScript({
        src: "analytics.google.com/api/v2/",
        onload: () => console.log("Script loaded")
    })

    if(loading) return <div>Script loading</div>
    if(error) return <div>Error occured</div>

    return (
        <div>
            ...
        </div>
    )
}
```

in this example, we want to add analytics to our component by loading this external script using useScript.
The load property indicates when the external script is done loading. We check the loading and error flag to display messages accordingly.

## useLocalStorage

This hook simplifies the storage and retrieval of data from the localStorage.
useLocalStorage is called with a key name. useLocalStorage returns three items in an array. The first is the value of the key name sent, the second is a function to set a new value to the key, and the third is a function to delete the key/value pair.