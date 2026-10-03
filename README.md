
# BSNL NOC SMS Auto Parser - TX + BTS

## What it does
- Auto receives SMS from BT-BSZNMS-S (BTS) and BX-OTNNOC-S (TX)
- Parses into 2 tabs
  - TX NODES: S.NO, NODE, TIME OF FAILURE, DOWN TIME, Restored, CPAN
  - BTS NODES: S.NO, NODE, TIME OF FAILURE (Create_Tm), SSA, TT ID, SEV, STATE
- Auto saves in Room DB, Export CSV

## How to build APK
1. Open folder bsnl_sms_app in Android Studio
2. Sync Gradle
3. Run on phone - Grant SMS permission
4. Incoming SMS auto parsed. No manual paste.

## Test without SMS
Send broadcast: adb shell am broadcast -a android.provider.Telephony.SMS_RECEIVE

## Parser logic same as web app you saw.
