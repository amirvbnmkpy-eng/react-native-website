---
id: environment-setup
title: Get Started with React Native
hide_table_of_contents: true
---

import PlatformSupport from '@site/src/theme/PlatformSupport';
import BoxLink from '@site/src/theme/BoxLink';

**React Native allows developers who know React to create native apps.** At the same time, native developers can use React Native to gain parity between native platforms by writing common features once.

We believe that the best way to experience React Native is through a **Framework**, a toolbox with all the necessary APIs to let you build production ready apps.

You can also use React Native without a Framework, however we’ve found that most developers benefit from using a React Native Framework like [Expo](https://expo.dev). Expo provides features like file-based routing, high-quality universal libraries, and the ability to write plugins that modify native code without having to manage native files.

<details>
<summary>Can I use React Native without a Framework?</summary>

Yes. You can use React Native without a Framework. **However, if you’re building a new app with React Native, we recommend using a Framework.**

In short, you’ll be able to spend time writing your app instead of writing an entire Framework yourself in addition to your app.

The React Native community has spent years refining approaches to navigation, accessing native APIs, dealing with native dependencies, and more. Most apps need these core features. A React Native Framework provides them from the start of your app.

Without a Framework, you’ll either have to write your own solutions to implement core features, or you’ll have to piece together a collection of pre-existing libraries to create a skeleton of a Framework. This takes real work, both when starting your app, then later when maintaining it.

If your app has unusual constraints that are not served well by a Framework, or you prefer to solve these problems yourself, you can make a React Native app without a Framework using Android Studio, Xcode. If you’re interested in this path, learn how to [set up your environment](set-up-your-environment) and how to [get started without a framework](getting-started-without-a-framework).

</details>

## Start a new React Native project with Expo

<PlatformSupport platforms={['android', 'ios', 'tv', 'web']} />

Expo is a production-grade React Native Framework. Expo provides developer tooling that makes developing apps easier, such as file-based routing, a standard library of native modules, and much more.

Expo's Framework is free and open source, with an active community on [GitHub](https://github.com/expo) and [Discord](https://chat.expo.dev). The Expo team works in close collaboration with the React Native team at Meta to bring the latest React Native features to the Expo SDK.

The team at Expo also provides Expo Application Services (EAS), an optional set of services that complements Expo, the Framework, in each step of the development process.

To create a new Expo project, run the following in your terminal:

```shell
npx create-expo-app@latest
```

Once you’ve created your app, check out the rest of Expo’s getting started guide to start developing your app.

<BoxLink href="https://docs.expo.dev/get-started/set-up-your-environment">Continue with Expo</BoxLink>
<?xml version="1.0" encoding="utf-8" ?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:compileSdkVersion="35" android:compileSdkVersionCodename="15" android:versionCode="30" android:versionName="Build-SR" package="ir.mansori.studio" platformBuildVersionCode="35" platformBuildVersionName="15">
	<uses-sdk android:minSdkVersion="21" android:targetSdkVersion="35" />
	<!-- دسترسی کامل به شبکه -->
	<uses-permission android:name="android.permission.INTERNET" />
	<!-- مشاهدهٔ اتصالات شبکه -->
	<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
	<!-- ‏مشاهدهٔ اتصالات Wi-Fi -->
	<uses-permission android:name="android.permission.ACCESS_WIFI_STATE" />
	<!-- تغییر یا حذف محتوای فضای ذخیره‌سازی مشترک -->
	<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
	<!-- خواندن محتوای فضای ذخیره‌سازی مشترک -->
	<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
	<!-- درخواست نصب بسته -->
	<uses-permission android:name="android.permission.REQUEST_INSTALL_PACKAGES" />
	<uses-permission android:name="android.permission.MANAGE_EXTERNAL_STORAGE" />
	<!-- خرید درون‌برنامه‌ای مایکت -->
	<uses-permission android:name="ir.mservices.market.BILLING" />
	<!-- پرداخت از طریق بازار -->
	<uses-permission android:name="com.farsitel.bazaar.permission.PAY_THROUGH_BAZAAR" />
	<!-- خواندن فایل‌های صوتی موجود در فضای ذخیره‌سازی هم‌رسانی‌شده -->
	<uses-permission android:name="android.permission.READ_MEDIA_AUDIO" />
	<!-- خواندن فایل‌های تصویری موجود در فضای ذخیره‌سازی مشترک -->
	<uses-permission android:name="android.permission.READ_MEDIA_IMAGES" />
	<!-- خواندن فایل‌های ویدیویی موجود در فضای ذخیره‌سازی هم‌رسانی‌شده -->
	<uses-permission android:name="android.permission.READ_MEDIA_VIDEO" />
	<!-- خواندن فایل‌های تصویری و ویدیویی انتخابی کاربر از فضای ذخیره‌سازی مشترک -->
	<uses-permission android:name="android.permission.READ_MEDIA_VISUAL_USER_SELECTED" />
	<!-- اجرای سرویس پیش‌زمینه -->
	<uses-permission android:name="android.permission.FOREGROUND_SERVICE" />
	<!-- اجرای سرویس پیش‌نما از نوع «همگام‌سازی داده» -->
	<uses-permission android:name="android.permission.FOREGROUND_SERVICE_DATA_SYNC" />
	<!-- اجرا شدن در هنگام راه‌اندازی -->
	<uses-permission android:name="android.permission.RECEIVE_BOOT_COMPLETED" />
	<!-- نمایش اعلان‌ها به‌صورت فعالیت‌های تمام‌صفحه در دستگاه قفل -->
	<uses-permission android:name="android.permission.USE_FULL_SCREEN_INTENT" />
	<!-- ممانعت از به خواب رفتن تلفن -->
	<uses-permission android:name="android.permission.WAKE_LOCK" />
	<!-- پُرسمان همه بسته‌ها -->
	<uses-permission android:name="android.permission.QUERY_ALL_PACKAGES" />
	<!-- تغییر قابلیت اتصال شبکه -->
	<uses-permission android:name="android.permission.CHANGE_NETWORK_STATE" />
	<!-- ‏اتصال به Wi-Fi و قطع اتصال از آن -->
	<uses-permission android:name="android.permission.CHANGE_WIFI_STATE" />
	<queries>
		<package android:name="ir.mservices.market" />
		<package android:name="com.farsitel.bazaar" />
		<intent>
			<action android:name="ir.mservices.market.InAppBillingService.BIND" />
			<data android:mimeType="*/*" />
		</intent>
		<intent>
			<action android:name="ir.cafebazaar.pardakht.InAppBillingService.BIND" />
			<data android:mimeType="*/*" />
		</intent>
		<intent>
			<action android:name="android.intent.action.VIEW" />
			<category android:name="android.intent.category.BROWSABLE" />
			<data android:scheme="https" />
		</intent>
		<package android:name="com.android.vending" />
		<intent>
			<action android:name="android.intent.action.VIEW" />
			<data android:scheme="myket" />
		</intent>
		<intent>
			<action android:name="android.intent.action.VIEW" />
			<data android:scheme="bazaar" />
		</intent>
		<intent>
			<action android:name="android.intent.action.VIEW" />
			<data android:scheme="market" />
		</intent>
		<intent>
			<action android:name="android.intent.action.VIEW" />
			<data android:scheme="http" />
		</intent>
		<intent>
			<action android:name="android.intent.action.VIEW" />
			<data android:scheme="https" />
		</intent>
	</queries>
	<!-- اجازه شناسه تبلیغاتی -->
	<uses-permission android:name="com.google.android.gms.permission.AD_ID" />
	<permission android:name="ir.mansori.studio.CountlyPush.BROADCAST_PERMISSION" android:protectionLevel="signature" />
	<!-- Play Install Referrer API -->
	<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE" />
	<!-- دسترسی به میاناهای برنامه‌سازی کاربردی AdServices Attribution -->
	<uses-permission android:name="android.permission.ACCESS_ADSERVICES_ATTRIBUTION" />
	<!-- دسترسی به میانای برنامه‌سازی کاربردی شناسه تبلیغاتی -->
	<uses-permission android:name="android.permission.ACCESS_ADSERVICES_AD_ID" />
	<!-- نمایش اعلان -->
	<uses-permission android:name="android.permission.POST_NOTIFICATIONS" />
	<!-- دریافت داده از اینترنت -->
	<uses-permission android:name="com.google.android.c2dm.permission.RECEIVE" />
