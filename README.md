TrivialDrive
============

	TRIVIAL DRIVE - SAMPLE FOR IN-APP BILLING VERSION 3
	Copyright (c) 2012 Google Inc. All rights reserved.
	Bruno Oliveira, 2012-11-29
	Reza Mohammadi, 2013-11-23
	Hamid Gharedaghi, 2013-12-02


CHANGELOG
---------

	2012-11-29: initial release
	2013-01-08: updated to include support for subscriptions
	2013-11-23: updating to include minor improvements in google's 5th release
	2013-12-02: updated to support Cando market in-app billing system


WHAT IS THIS SAMPLE?
--------------------

   This game is a simple "driving" game where the player can buy gas
   and drive. The car has a tank which stores gas. When the player purchases
   gas, the tank fills up (1/4 tank at a time). When the player drives, the gas
   in the tank diminishes (also 1/4 tank at a time).

   The user can also purchase a "premium upgrade" that gives them a red car
   instead of the standard blue one (exciting!).

   The user can also purchase a subscription ("infinite gas") that allows them
   to drive without using up any gas while that subscription is active.


HOW TO RUN THIS SAMPLE
----------------------

   This sample can't be run as-is. You have to create your own
   application instance in the Developer Console and modify this
   sample to point to it.


PERMISSIONS
----------------------

	1. Cando:
		in-app billing doesn't need any permissions.
	2. Bazzar:
		<uses-permission android:name="com.farsitel.bazaar.permission.PAY_THROUGH_BAZAAR" />
	3. Play:
		<uses-permission android:name="com.android.vending.BILLING" />


A NOTE ABOUT SECURITY
---------------------

   This sample app implements signature verification but does not demonstrate
   how to enforce a tight security model. When releasing a production application 
   to the general public, we highly recommend that you implement the security best
   practices described in Google documentation at:

	http://developer.android.com/google/play/billing/billing_best_practices.html

   In particular, you should set developer payload strings when making purchase
   requests and you should verify them when reading back the results. This will make
   it more for a malicious party to perform a replay attack on your app.
