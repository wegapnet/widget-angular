# 💬 Wegap Widget for Angular / ویجت ویگپ برای Angular

This repository contains the official Angular version of the Wegap widget.  
این مخزن شامل نسخه رسمی ویجت ویگپ برای برنامه‌های Angular است. با استفاده از این ویجت می‌توانید قابلیت‌هایی مانند **چت، تماس صوتی/تصویری و دانشیار هوش مصنوعی** را به راحتی به اپلیکیشن خود اضافه کنید.

---

## 📦 Installation / نصب

```bash
npm install @wegapnet/widget-angular
```

---

## 🚀 Quick Usage / استفاده سریع

در فایل ماژول:

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent } from './app.component';
import { WegapWidgetModule } from '@wegapnet/widget-angular';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule, WegapWidgetModule],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

در فایل کامپوننت:

```ts
@Component({
  selector: 'app-root',
  template: \`
    <wegap-widget
      [authKey]="'YOUR_AUTH_KEY'"
      [theme]="'light'"
      [position]="'bottom-right'"
      [language]="'fa'">
    </wegap-widget>
  \`
})
export class AppComponent { }
```

---

## ⚙️ Config Options / تنظیمات

| Prop Name | Type   | Description EN                                      | توضیح فارسی |
|-----------|--------|------------------------------------------------------|--------------|
| authKey   | string | Your unique authentication key                      | کلید احراز هویت شما |
| theme     | string | Theme mode: `light` or `dark`                       | تم: روشن یا تیره |
| position  | string | Widget position: `bottom-right`, `bottom-left`, etc | موقعیت ویجت |
| language  | string | Default widget language (fa, en, ar, ...)           | زبان پیش‌فرض |

---

## 📄 Documentation / مستندات کامل

- [See full guide in Wegap Wiki](https://wegap.net/wiki/angular/نصب-و-راه-اندازی/راهنمای-ویجت-ویگپ/دانشیار-ویگپ-id-8914)
- مشاهده راهنما در ویکی ویگپ ↑
