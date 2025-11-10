# Complete EmailJS Setup Instructions
## Service ID: service_gu7350o

Your portfolio is already configured with **Service ID: service_gu7350o**

## What You Need to Complete:

You need to provide 2 more values:
1. ✅ **Service ID** - Already set: `service_gu7350o`
2. ⚠️ **Template ID** - You need to create this
3. ⚠️ **Public Key** - You need to get this from your EmailJS account

---

## Step 1: Get Your Public Key (2 minutes)

1. Log into your EmailJS account at https://dashboard.emailjs.com/
2. Click on **"Account"** in the left sidebar
3. Find the **"API Keys"** section
4. Copy your **Public Key** (it looks like: `AbCdEfGh1234567`)
5. Save this for Step 3

---

## Step 2: Create Email Template (5 minutes)

### A. Create New Template
1. In EmailJS dashboard, go to **"Email Templates"**
2. Click **"Create New Template"**

### B. Configure Template Settings

**Template Name:** `Portfolio Contact`

**From Name:** `Portfolio Website`

**To Email:** `saiprasad.jnv@gmail.com` (or your preferred email)

**Subject:** `New Message from {{from_name}} - Portfolio Contact`

### C. Template Content (Copy this EXACTLY)

```html
<div style="font-family: Arial, sans-serif; max-width: 600px; margin: 0 auto;">
    <div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 20px; border-radius: 10px 10px 0 0;">
        <h2 style="margin: 0;">New Portfolio Contact</h2>
    </div>
    
    <div style="background: #f9f9f9; padding: 20px; border-radius: 0 0 10px 10px; border: 1px solid #e0e0e0;">
        <h3>Contact Information:</h3>
        <p><strong>Name:</strong> {{from_name}}</p>
        <p><strong>Email:</strong> {{from_email}}</p>
        
        <h3>Message:</h3>
        <div style="background: white; padding: 15px; border-radius: 5px; border: 1px solid #ddd;">
            <p>{{message}}</p>
        </div>
        
        <hr style="margin: 20px 0; border: none; border-top: 1px solid #ddd;">
        <p style="color: #999; font-size: 12px;">This email was sent from your portfolio contact form.</p>
    </div>
</div>
```

### D. Save and Get Template ID
1. Click **"Save"** button
2. Your **Template ID** will be displayed (looks like: `template_xyz123`)
3. **Copy this Template ID** - you'll need it in Step 3

---

## Step 3: Update Your Portfolio Code

Open your `advanced-portfolio.jsx` file and find these lines (around line 25-28):

```javascript
// EmailJS Configuration
const EMAILJS_SERVICE_ID = 'service_gu7350o'; // Your EmailJS Service ID
const EMAILJS_TEMPLATE_ID = 'YOUR_TEMPLATE_ID'; // Replace with your template ID from EmailJS dashboard
const EMAILJS_PUBLIC_KEY = 'YOUR_PUBLIC_KEY'; // Replace with your public key from EmailJS dashboard
```

**Replace with your actual values:**

```javascript
// EmailJS Configuration
const EMAILJS_SERVICE_ID = 'service_gu7350o';
const EMAILJS_TEMPLATE_ID = 'template_XXXXXXX'; // Paste your Template ID here
const EMAILJS_PUBLIC_KEY = 'XXXXXXXXXXXXXXX'; // Paste your Public Key here
```

### Example (with fake values):
```javascript
// EmailJS Configuration
const EMAILJS_SERVICE_ID = 'service_gu7350o';
const EMAILJS_TEMPLATE_ID = 'template_abc123';
const EMAILJS_PUBLIC_KEY = 'XyZ9AbC8dEf7GhI';
```

---

## Step 4: Test Your Contact Form

1. Open your portfolio website
2. Scroll to the **Contact** section
3. Fill out the form:
   - **Name:** Test User
   - **Email:** your.email@example.com
   - **Message:** This is a test message
4. Click **"Send Message"**
5. You should see:
   - A loading spinner
   - Then a green success message: ✓ "Message sent successfully!"
6. Check your email inbox for the message

---

## Troubleshooting

### ❌ Error: "Failed to send email"

**Possible Causes:**
1. Template ID is incorrect
2. Public Key is incorrect
3. Service ID is not active
4. Template variables don't match

**Solutions:**
1. Double-check all three IDs in your code
2. Make sure template uses these exact variable names:
   - `{{from_name}}`
   - `{{from_email}}`
   - `{{message}}`
3. Verify your EmailJS service is connected and active
4. Check browser console (F12) for detailed error messages

### ❌ Form doesn't submit

**Check:**
1. All form fields are filled
2. Email format is valid
3. JavaScript console for errors
4. Internet connection is active

### ❌ Email goes to spam

**Solutions:**
1. Mark the email as "Not Spam" in your inbox
2. Add your EmailJS sending email to contacts
3. Use a custom domain email (paid EmailJS feature)

---

## Verification Checklist

Before testing, verify:

- [ ] Service ID is set to: `service_gu7350o`
- [ ] Template ID is copied from EmailJS dashboard
- [ ] Public Key is copied from EmailJS dashboard
- [ ] Template uses correct variable names (from_name, from_email, message)
- [ ] Email service is connected in EmailJS dashboard
- [ ] Template is saved and active

---

## What's Already Working in Your Portfolio

✅ Form validation (all fields required)
✅ Email format validation
✅ Loading state with spinner
✅ Success message display (green notification)
✅ Error message display (red notification)
✅ Automatic message clearing (after 5 seconds)
✅ Form reset after successful send
✅ Button disabled during submission

---

## Quick Reference

**Your Configuration:**
```
Service ID:  service_gu7350o  ✅ (Already set)
Template ID: [Need to add]     ⚠️
Public Key:  [Need to add]     ⚠️
```

**EmailJS Dashboard:** https://dashboard.emailjs.com/
**Documentation:** https://www.emailjs.com/docs/

---

## Need Help?

1. Check EmailJS documentation: https://www.emailjs.com/docs/
2. Check browser console for errors (F12 key)
3. Verify all IDs are correctly copied (no extra spaces)
4. Test the template in EmailJS dashboard first
5. Make sure you're logged into EmailJS

---

## Free Tier Limits

- 200 emails per month
- 2 email services
- Unlimited templates
- Basic support

If you need more, upgrade at: https://www.emailjs.com/pricing

---

**Status:** 🟡 Setup 33% Complete (Service ID configured)
**Next Step:** Create template and get Template ID + Public Key
**Time Required:** ~5 minutes to complete setup
