const express = require('express');
const app = express();
const port = process.env.PORT || 3000;

// Middleware za parsiranje JSON tijela zahtjeva
app.use(express.json());

// Ruta za POST zahtjeve
app.post('/data', (req, res) => {
    console.log('Received data:', req.body);
    res.status(200).send('Data received');
});

// Ruta za GET zahtjeve (ako želite obraditi GET zahtjeve na rootu)
app.get('/', (req, res) => {
    res.send('Hello World!');
});

// Pokretanje servera
app.listen(port, () => {
    console.log(`Server running on http://localhost:${port}`);
});
