# DR-001: SMS verification code not delivered at registration; “Resend code” button hangs

## Summary
When a new user enters their phone number during sign‑up, the app fails to send the SMS code. After the 60‑second timer expires, tapping **Resend SMS** displays a perpetual loading spinner, but the SMS still does not arrive.

## Environment
- **Device:** iPhone 14 Pro Max  
- **OS:** iOS 18.5  
- **Network:** Wi‑Fi  

## Steps to Reproduce
1. Choose your country code  
2. Write down your phone number  
3. Tap **Go**  
4. Verify the CAPTCHA  
5. Observe that no SMS arrives  
6. Wait until the 60‑second countdown ends  
7. Tap **Resend SMS**  
8. Observe the spinner runs indefinitely and no SMS is received.

## Expected Result
1. An SMS with the verification code is delivered within a few seconds.  
2. If the user taps **Resend SMS** after the timer expires, a new SMS is sent.

## Actual Result
1. No SMS is ever delivered.  
2. **Resend SMS** shows a never‑ending loading spinner without sending anything.

## Severity & Priority
- **Severity:** High (blocks user registration)  
- **Priority:** P1
