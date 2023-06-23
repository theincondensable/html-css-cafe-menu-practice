# SYNTAX OF Type-Selectors Styling: <element> { <style>: <properties>; }

### 1: You can style the elements inside the <head> of the HTML document.
like this:
    `   p {
            text-align: center;
        }

        or you can group so many with a single styling form like this:
        h1, h2, p {
            text-align: center;
        }`

### 2: You have styled three elements by writing CSS inside the style tags. This works, but since there will be many more styles, it's best to put all the styles in a separate file and link to it.
We have created a separate styles.css file for you and switched the editor view to that file. You can change between files with the tabs at the top of the editor.

### 3: HOW TO LINK THE CSS TO HTML?
inside the <head> of the HTML document, use the self-closing <link> with its two attributes set to:
    1. href="<the directory of your CSS file>"
    2. rel="stylesheet"

DONE! :)

### 4: For the styling of the page to look similar on MOBILE as it does on a DESKTOP or LAPTOP, you need to add a meta element with a special content attribute.
<meta name="viewport" content="width=device-width, initial-scale=1.0">

### 5: <div> element is mainly used for designing Layout purposes unlike unlike the other content elements you have used so far.
up until now, move all the body parts, into a <div> element.

we can style the <div> separately so that this DIV element is only affected with our style. like:
div {
    width: 300px; (or we can say 80% which means 80% of the PARENT ELEMENT, so that if the parent is BODY ....)
    background-color: burlywood; 
}
for now, for centering the <div> element inside its PARENT which is <body>, we use this:
div {
    ...
    margin-left: auto;
    margin-right: auto;
}

### 6: Syntax of Class-Selector Styling: .class-name { styles }
first you have to define your let's say <div> element a Class name:
    <div class="menu"> for example.
    then inside your CSS:
    .menu {
        ...
    }

### 7: if the font-family of some specific Font is not available/found, you can specify a Fallback value:
h1, h2 {
    font-family: Impact, **serif**
}
now the "serif" is the Fallback option, if the "Impact" is not available/found, then "serif" is applied.