# graduate_project_99-s
졸업프로젝트(React button 연습)
<!DOCTYPE html>
<html>
    <body>
    <div id="root"></div>
    </body>
    <script src="https://unpkg.com/react@17.0.2/umd/react.production.min.js"></script>
    <script src="https://unpkg.com/react-dom@17.0.2/umd/react-dom.production.min.js"></script>
   <script>
    const root = document.getElementById("root");
    const h3 = React.createElement(
        "h3", 
    {
        onMouseEnter: () => console.log("mouse enter"),
    }, 
    "Hello I'm a span"
    );
    const btn = React.createElement(
        "button",
        {
            onClick: ()=> console.log("im clicked"),
        },
        "Click me"
    );
    const container = React.createElement("div", null, [h3, btn]);
    ReactDOM.render(container, root);
   </script>
</html>
