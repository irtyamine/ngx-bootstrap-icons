<p align="center" style="text-align:center">
  <a href="https://v5.getbootstrap.com/">
    <img src="https://v5.getbootstrap.com/docs/5.0/assets/brand/bootstrap-logo-shadow.png" alt="Bootstrap logo" width="200" height="165">
  </a>
  <h3 align="center">ngx-bootstrap-icons</h3>
</p>

### This Angular module allows you to use the Bootstrap Icons in your angular application.
<br />

[![GitHub issues](https://img.shields.io/github/issues/avmaisak/ngx-bootstrap-icons)](https://github.com/avmaisak/ngx-bootstrap-icons/issues)
[![GitHub license](https://img.shields.io/github/license/avmaisak/ngx-bootstrap-icons)](https://github.com/avmaisak/ngx-bootstrap-icons/blob/master/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/avmaisak/ngx-bootstrap-icons)](https://github.com/avmaisak/ngx-bootstrap-icons/stargazers)
[![npm version](https://badge.fury.io/js/ngx-bootstrap-icons.svg)](https://badge.fury.io/js/ngx-bootstrap-icons)
[![Package Quality](https://npm.packagequality.com/shield/ngx-bootstrap-icons.svg)](https://packagequality.com/#?package=ngx-bootstrap-icons) 
 <a href="https://www.figma.com/file/hTJtQ2MrMTeNVmYrVBqNZZ/Bootstrap-Icons-v1.0.0-alpha5?node-id=0%3A1" target="_blank">
    <img src="https://avatars3.githubusercontent.com/u/5155369?s=200&v=4" alt="Bootstrap logo" width="21" height="21">
  </a>

<br />

![Bootstrap Icons full set](https://user-images.githubusercontent.com/98681/85891337-be640680-b7a3-11ea-84a0-0a103fce118c.png)


### Demo

<a href="https://avmaisak.github.io/ngx-bootstrap-icons/" align="center"><strong>Demo Here</strong></a>

### Usage

_1. Install the package_

```sh
npm i ngx-bootstrap-icons --save
```
_2. Import module_

```ts  
import { NgxBootstrapIconsModule } from 'ngx-bootstrap-icons';
```

_3. Import assets_

You can import all icons (not recomended) or each icon individually.

_3.1 Import all icons_

```ts
import { allIcons } from 'ngx-bootstrap-icons';
```

_3.2 Import some icons_
```ts
import { Alarm, AlarmFill, AlertCircle } from 'ngx-bootstrap-icons';
// Select some icons (use an object, not an array)
const icons = {
  Alarm,
  AlarmFill,
  AlertCircle
};
```

_4. Import Module (all icons)_

```ts
import { NgxBootstrapIconsModule, allIcons } from 'ngx-bootstrap-icons';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule,
    NgxBootstrapIconsModule.pick(allIcons)
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

```
_4.1. Import Module (some icons)_

```ts
import { NgxBootstrapIconsModule } from 'ngx-bootstrap-icons';
import { Alarm, AlarmFill, AlertCircle } from 'ngx-bootstrap-icons';

// Select some icons (use an object, not an array)
const icons = {
  Alarm,
  AlarmFill,
  AlertCircle
};

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule,
    NgxBootstrapIconsModule.pick(icons)
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

_5. Use it in template_
```ts
<i-bs name="alarm-fill"></i-bs>
```
Also you can use width and height for icon (By default width and height are 1rem)
```ts
<i-bs 
  name="alarm-fill" 
  width="2rem" 
  height="2rem">
</i-bs>
```
