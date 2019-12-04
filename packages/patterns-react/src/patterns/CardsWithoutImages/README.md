# Cards without images

> The Cards without images pattern is to be utilized within IBM.com.

## Getting started

Here's a quick example to get you started.

```scss
// yourapplication.scss
@import '@carbon/type/scss/font-face/mono';
@import '@carbon/type/scss/font-face/sans';
@include carbon--font-face-mono();
@include carbon--font-face-sans();
```

> 💡 Only import font's once per usage

```javascript
import React from 'react';
import ReactDOM from 'react-dom';
import { CardsWithoutImages } from '@carbon/ibmdotcom-patterns-react';
import 'yourapplication.scss';
import '@carbon/ibmdotcom-styles/scss/patterns/cards-without-images/index.scss';

function App() {
  return;
  <CardsWithoutImages cardsGroup={cardsGroup} />;
}

ReactDOM.render(<App />, document.querySelector('#app'));
```

> 💡 Don't forget to import the cards-without-images styles from
> [@carbon/ibmdotcom-styles](https://github.com/carbon-design-system/ibm-dotcom-library/blob/master/packages/styles).

#### Feature Flags

To utilize the following features, set the following variable's to `true` within
your `.env` file or your application build settings.

```
DDS_CARDS_WITHOUT_IMAGES=true
```

> See
> [feature-flags.md](https://github.com/carbon-design-system/ibm-dotcom-library/blob/master/packages/patterns-react/docs/feature-flags.md)
> and
> [.env.example](https://github.com/carbon-design-system/ibm-dotcom-library/blob/master/packages/patterns-react/.env.example)
> for more information

## cardsGroup ( Array of Objects )

| Name        | Description                                                  |
| ----------- | ------------------------------------------------------------ |
| `title`     | Cards without images title                                   |
| `groupCard` | groupCard, array with href, text and target properties       |
| `cards`     | Cards, array of objects with title, copy and link properties |

## Stable selectors

| Name                                                  | Description |
| ----------------------------------------------------- | ----------- |
| `dds--cards-without-images`                           | Component   |
| `dds--cards-without-images-group`                     | Component   |
| `dds--cards-without-images-group__card-${card.title}` | Component   |

## 🙌 Contributing

We're always looking for contributors to help us fix bugs, build new features,
or help us improve the project documentation. If you're interested, definitely
check out our
[Contributing Guide](https://github.com/carbon-design-system/ibm-dotcom-library/blob/master/.github/CONTRIBUTING.md)!
👀

## 📝 License

Licensed under the
[Apache 2.0 License](https://github.com/carbon-design-system/ibm-dotcom-library/blob/master/LICENSE).