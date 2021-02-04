# verticaltabpanels
VerticalTabPanels is a Vuetify UI component for vertically displaying the v-tabs component's content panels. The design is commonly seen in food ordering apps for displaying food menus.

## Features
### Smooth scroll to a tab panel
 When the user clicks a tab, VerticalTabPanels will scroll 
 the page to its corresponding panel with an effect.

### Switch tabs on scroll
 When the user scrolls through the tab panels, the active tab
 of the v-tabs component will be accordingly changed.
 
## Usage
 1. Declare the VerticalTabPanels component as a sibling of
 the v-tabs component.

 2. Set a series of content blocks (e.g. div or v-card)
 inside <VerticalTabPanels></VerticalTabPanels> as tab panels.
 The number of panels should be the same as the number of tabs.

 3. Inside the v-tabs component's "change" event handler, 
 emit an event named "scrollToPanel" (here we use an event bus), 
 with a tab index value, for example:
   this.$bus.$emit("scrollToPanel", index);

## Required Parameters
 * v-model: the v-tabs component and the VerticalTabPanels
 component share the same integer variable as their v-model
 value. The variable represents the index of the active tab.

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
