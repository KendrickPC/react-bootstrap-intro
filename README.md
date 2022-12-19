# React Bootstrap Tutorial:

1. In console, create a new project
```console
npx create-react-app react-bootstrap-tutorial
```

2. Install bootstrap with NPM
[React Bootstrap Documentation](https://react-bootstrap.github.io/getting-started/introduction/)
```console
npm install react-bootstrap bootstrap
```

3. Start react application
```console
npm start
```

4. Inside src/app.js, import Button
```js
import Button from 'react-bootstrap/Button';
```
5. Render Button on page src/app.js
```js
import './App.css';
import Button from 'react-bootstrap/Button';
function App() {
  return (
    <div className="App">
      // No styling yet.
      // Right click, inspect, check Bootstrap classes.
      <Button>Click Me for SPAM</Button>
    </div>
  );
}

export default App;

```
6. Import Bootstrap CSS for styling.
   Button style should now be changed. =)
```js
import 'bootstrap/dist/css/bootstrap.min.css'
```
7. There are two different ways to import our button.
```js
// Only importing the Button way.
import Button from 'react-bootstrap/Button';
// Importing the Button with the entire bootstrap library.
import {Button} from 'react-bootstrap'
```
8. Add an alert.
```js
import {Button, Alert} from 'react-bootstrap'

<Alert>Chat GPT 4ever!!!</Alert>
<Button>Click Me for SPAM</Button>
```
9. Change alert color
```js
<Alert variant="success">Chat GPT 4ever!!!</Alert>
```

10. Breadcrumbs:
```js
import './App.css';
import { Button, Alert, Breadcrumb } from 'react-bootstrap'
import 'bootstrap/dist/css/bootstrap.min.css'
function App() {
  return (
    <div className="App">
      <header className="App-header">
        <Breadcrumb>
          <Breadcrumb.Item>BTS</Breadcrumb.Item>
          <Breadcrumb.Item>BTS</Breadcrumb.Item>
          // Grays out last item.
          <Breadcrumb.Item active="true">BTS</Breadcrumb.Item>
        </Breadcrumb>
        <Alert variant="success">Chat GPT 4ever!!!</Alert>
        <Button>Click Me for SPAM</Button>
      </header>
    </div>
  );
}

export default App;
```

11. Let's make a CARD.
```js
import { Button, Alert, Breadcrumb, Card } from 'react-bootstrap'

<Card>
  <Card.Img />
  <Card.Body>
    <Card.Title>Yu Gi Oh</Card.Title>
    <Card.Text>Best Card Game EVER!</Card.Text>
    <Button variant="warning">Yu Gi Oh BUTTON!</Button>
  </Card.Body>
</Card>
```

12. Bootstrap is being overwritten by React app's color.
```js
import { Button, Alert, Breadcrumb, Card } from 'react-bootstrap'

<Card style={{style: "pink"}}>
  <Card.Img />
  <Card.Body>
    <Card.Title>Yu Gi Oh</Card.Title>
    <Card.Text>Best Card Game EVER!</Card.Text>
    <Button variant="warning">Yu Gi Oh BUTTON!</Button>
  </Card.Body>
</Card>
```

13. Image added into Card component
```js
<Card style={{style: "pink"}}>
  <Card.Img src="https://prod-ripcut-delivery.disney-plus.net/v1/variant/disney/8D1B259B4E54353EC4BF0A4AFC3A83D30D79EEDE01BA1D15CD34E0CA25F98E41/scale?width=1200&aspectRatio=1.78&format=jpeg" />
  <Card.Body>
    <Card.Title>Yu Gi Oh</Card.Title>
    <Card.Text>Best Card Game EVER!</Card.Text>
    <Button variant="warning">Yu Gi Oh BUTTON!</Button>
  </Card.Body>
</Card>
```

14. Add a margin bottom:
```js
<Card className="mb-3" style={{style: "pink"}}>
```

15. Make a form. YOu do!
16. Make a Navbar.

17. Make a container.
[Bootstrap Grid System](https://getbootstrap.com/docs/4.0/layout/grid/)