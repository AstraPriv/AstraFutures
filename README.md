# 📱 Astra Futures SMS Notifications Guide

Get real-time trading signals delivered directly to your phone via SMS.

## 🔔 How to Opt-In to SMS Notifications

### Prerequisites
- Must be a paid subscribers of Astra Futures trading group. Visit AstraBlock.io to subscribe. 
- Have access to the Telegram bot
- Valid phone number with SMS capability

### Step-by-Step Opt-In Process

1. **Join the Trading Channel**
   - Ensure your membership is active by joining the private telegram group channel.
   - Start @AstraFutures_bot on telegram by DMing the bot and clicking "Start" 
   - The system verifies your membership before allowing SMS registration

2. **Start SMS Registration**
   ```
   /register_sms +1234567890
   ```
   - Replace `+1234567890` with your phone number
   - Use international format (include country code with +)
   - Examples: `+14155551234` (US), `+447700900123` (UK)

3. **Verify Your Phone Number**
   - You'll receive a 6-digit verification code via SMS
   - Enter the code using:
   ```
   /verify_sms 123456
   ```
   - Replace `123456` with your actual verification code

4. **Welcome SMS**
   - Once verified, you'll receive a welcome text message
   - SMS alerts are automatically enabled for all trading signals

## 📊 Check Your SMS Status

To check if SMS notifications are active:
```
/sms_status
```

This will show you:
- ✅ SMS alerts active
- ⏳ Phone number not verified  
- ⚠️ SMS disabled - not a channel member
- 🔇 SMS alerts disabled

## 🔕 How to Opt-Out of SMS Notifications

### Option 1: Disable SMS Alerts (Keep Registration)
```
/sms_disable
```
- Keeps your phone number registered
- Stops all SMS notifications
- Can be re-enabled later with `/sms_enable`

### Option 2: Complete Removal
```
/sms_remove
```
- Completely removes your phone number from the system
- Deletes all SMS registration data
- Requires full re-registration to opt back in

### Option 3: Reply to SMS
You can also reply to any SMS message with:
```
STOP
```
- Standard SMS opt-out method
- Automatically disables SMS alerts

## 🔄 Re-Enable SMS Alerts

If you previously disabled SMS alerts:
```
/sms_enable
```
- Only works if you're still a channel member
- Reactivates SMS notifications immediately

## ⚠️ Important Notes

- **Channel Membership Required**: SMS alerts are automatically disabled if you leave the trading channel
- **Verification Expires**: Verification codes expire after 1 hour
- **One Phone Per User**: Each phone number can only be registered once
- **Rate Limits**: The system may rate-limit requests to prevent spam

## 🛠️ Troubleshooting

### "Invalid phone number format"
- Ensure you're using international format: `+countrycode-number`
- Remove any spaces, dashes, or special characters except `+`

### "You must be a member of the trading channel"
- Verify you're still a member of the Astra Futures channel
- Rejoin the channel if you were removed

### "No pending verification found"
- Verification codes expire after 1 hour
- Start over with `/register_sms` if expired

### "This phone number is already registered"
- Each phone number can only be used once
- Contact support if you need to change your registered number

## 💡 SMS Message Format

You'll receive concise trading signals like:
```
🟢 BTC LONG
📊 $45,250 | SL: $44,800
🎯 T1:46.2K T2:47.1K T3:48.5K
Conv: 8/10 | 14:30
```

## 📞 Support

For technical issues or questions:
- Check `/sms_status` first
- Contact the Astra Futures support team
- Review this guide for common solutions

---

> **Privacy Notice**: Your phone number is only used for SMS trading alerts and is never shared with third parties.
