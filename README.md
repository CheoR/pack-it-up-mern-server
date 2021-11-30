<img src="./assets/images/PackItUpLogo.png" alt="Pack It Up Logo" />

# PackItUpMern

[PackItUpMern] is my frontend capstone project redone using the MERN stack.

The original [PackItUp](https://cr-demo--packitup.netlify.app) is a moving/storage CRUD app created with

- React
- HTML
- CSS
- Fetch API
- json-server

to help users inventorize items they pack into boxes for moving/storage.

[![V1 Demo](https://img.shields.io/badge/Live%20Demo-PackItUp-green)](https://cr-demo--packitup.netlify.app), [github](https://github.com/CheoR/pack-it-up-api) repo.

Initial design made with Figma and the entity relational diagram made with diagramdb.io.

Issue tickets follow [BDD](https://en.wikipedia.org/wiki/Behavior-driven_development#Behavioral_specifications), Behavior-Driven Development and use Github Project board to track issue lifecyles.

Old Sever-side repo [here](https://github.com/CheoR/pack-it-up-api).

New client-side MERN repo [here](https://github.com/CheoR/pack-it-up-mern-client).

# About Me

Hi, my name's Cheo.

This is my front-end capstone project for Nashville Software School.

[![Demo](https://img.shields.io/badge/Live%20Demo-PackItUp-green)](https://cr-demo--packitup.netlify.app/)

## 🔗 Links

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://cheor.github.io/portfolio/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/cheo-roman/)

## Table of contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Endpoints](#endpoints)
- [Demo](#demo)
- [ERD](#erd)
- [Layout](#layout)
- [Cloning](#cloning)
- [Running Tests](#running-tests)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Features

- [ ] User should be able to add/remove/update item(s).

- [ ] User should be able to add/remove/update box(es).

- [ ] User should be able to add/remove/update move(s).

- [ ] User should be able to link/delink items from boxes.

- [ ] User should be able to link/delink boxes from moves.

- [ ] User should not be able to modifiy other user's information.

- [ ] User should be able to save their moves, boxes, items.

- [ ] User should be able to authenticate.

- [ ] User should only be able to add/remove/edit boxes, items if they are logged in.

- [ ] Boxes should automatically aggregate and update its information pertaining to its contents.

- [ ] Moves should automatically aggregate and update its information pertaining to its boxes' contents.

## Tech Stack

1. Mongo
2. Express
3. React
4. Node
5. Material-UI

## Endpoints

- /user
- /moves
- /moves/${id}
- /boxes
- /boxex/${id}
- /items
- /items/${id}

## Demo

<img src="./assets/screen-recording.gif" alt="Pack It Up App Demo">

## ERD

Entity relationship diagram can be viewd at [diagram](https://dbdiagram.io/d/603cf260fcdcb6230b21ffe2) or latest screen capture below.

<details>
  <img src="./assets/images/PackItUp.png" alt="entity relationship diagram for pack it up" />
</details>

## Layout

Most up to date layout can be viewd at [my figma layout](https://www.figma.com/file/FVTItU8oORU8Mrihcd60Jj/PackItUp?node-id=39%3A0) or you can view latest screen capture below:

<details>
 <img src="./assets/images/Layout.png" alt="layout for pack it up" />
</details>

## Cloning

```bash
git clone git@github.com:CheoR/pack-it-up-mern-server.git
cd pack-it-up-mern
npm install
```

## Running Tests

After forking the repo.

```bash

git fetch --all
git checkout <branch-name>
npm install
npm start

```

In another tab, cd into `api` and run

`json-server -p 8088 database.json`

Please note, as of right now, running the above command including `-w` would cause json-serve to crash if user chooses to create 4 or more objects at once through the `ADD` button.

## Roadmap

- [_] Encode item/box/move data as a QR code that can be printed out as a label for shipping.
- [_] Add a complentary QR decoding, so user can scan QR on a box and get information about its contents (if user has authorization). User can limit what data 3rd parties (movers, storage management, ect) can see.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

Please fill out the template for pulll request and label them appropriately.

## Acknowledgements

Thanks to NSS and everybody in my cohert that has helped me figure out problems when I was overthinking it.

## License

[MIT](https://choosealicense.com/licenses/mit/)
