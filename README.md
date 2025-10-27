# Getting Started with Syncfusion® Barcode Component in Vue 3

This sample project demonstrates how to use the Syncfusion Barcode, QR Code and DataMatrix generator components in a Vue 3 application.

The repository contains a minimal Vue 3 app (created with Vue CLI) that registers and renders the following Syncfusion components from `@syncfusion/ej2-vue-barcode-generator`:

- BarcodeGeneratorComponent (`<ejs-barcodegenerator>`)
- QRCodeGeneratorComponent (`<ejs-qrcodegenerator>`)
- DataMatrixGeneratorComponent (`<ejs-datamatrixgenerator>`)

## Prerequisites

[System requirements for Syncfusion® Vue UI components](https://ej2.syncfusion.com/vue/documentation/system-requirements/)

## Creating Vue application using Vue CLI

The easiest way to create a Vue application is to use the [`Vue CLI`](https://github.com/vuejs/vue-cli). Vue CLI versions higher than [`4.5.0`](https://v3.vuejs.org/guide/migration/introduction.html#vue-cli) are mandatory for creating applications using Vue 3. Use the following command to uninstall older versions of the Vue CLI.

```bash
npm uninstall vue-cli -g
```

Use the following commands to install the latest version of Vue CLI.

```bash
npm install -g @vue/cli
npm install -g @vue/cli-init
```

Create a new project using the following command.

```bash
vue create quickstart

```

Initiating a new project prompts us to select the type of project to be used for the current application. Select the option `Default (Vue 3)` from the menu.


## Adding Syncfusion® Barcode package in the application

Use the following command to install it.

```bash
npm install @syncfusion/ej2-vue-barcode-generator
```

## Adding CSS reference for Syncfusion® Vue Barcode component

Import the necessary css styles for the Barcode component along with dependency styles in the `<style>` section of the `src/App.vue` file as follows.

```
<style>
  @import "../node_modules/@syncfusion/ej2-base/styles/material.css";
  @import "../node_modules/@syncfusion/ej2-icons/styles/material.css";
  @import "../node_modules/@syncfusion/ej2-vue-barcode-generator/styles/material.css";
</style>
```

- The example sets some simple properties (width, height, value, type, mode, displayText) and renders each generator with the corresponding tag:

## Running the application

Run the application using the following command.

```bash
npm run serve
```

Open http://localhost:8080 in your browser (Vue CLI's default dev server) to see the sample.

