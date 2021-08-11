<template>
<div id="app1">
        <ejs-barcodegenerator
            id="barcode"
            ref="barcodeControl"
            :width="width"
            :height="height"
            :type="type"
            :displayText="displaytext"
            :value="value"
            :mode="mode"
        >
        </ejs-barcodegenerator>
    </div>
    <div id="app" class="barcodeStyle">
        <ejs-datamatrixgenerator
            id="qrcode"
            ref="qrcodeControl"
            :width="width"
            :height="height"
            :type="type"
            :displayText="displaytext"
            :value="value"
            :mode="mode"
        >
        </ejs-datamatrixgenerator>
    </div>
    <div id="app" class="barcodeStyle">
        <ejs-qrcodegenerator
            id="qrcode"
            ref="qrcodeControl"
            :width="width"
            :height="height"
            :type="type"
            :displayText="displaytext"
            :value="value"
            :mode="mode"
        >
        </ejs-qrcodegenerator>
    </div>
</template>

<script>

import { BarcodeGeneratorComponent, QRCodeGeneratorComponent, DataMatrixGeneratorComponent } from '@syncfusion/ej2-vue-barcode-generator';

import "../node_modules/@syncfusion/ej2-base/styles/material.css";
import "../node_modules/@syncfusion/ej2-icons/styles/material.css";
import "../node_modules/@syncfusion/ej2-vue-barcode-generator/styles/material.css";

export default {
  name: "App",
  components: {
    "ejs-datamatrixgenerator": DataMatrixGeneratorComponent,
    "ejs-qrcodegenerator": QRCodeGeneratorComponent,
    "ejs-barcodegenerator": BarcodeGeneratorComponent
  },
  data() {
    return {
      width: "200px",
        height: "150px",
        type: "Codabar",
        value: "123456789",
        mode: "SVG",
        displaytext: { text: 'Syncfusion' },
    };
  },
};
</script>