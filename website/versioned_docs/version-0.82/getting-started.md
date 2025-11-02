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
