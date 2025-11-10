# 📋 COPY-PASTE READY EMAIL TEMPLATE
## For EmailJS Dashboard - Service: service_gu7350o

═══════════════════════════════════════════════════════════════

## STEP-BY-STEP TEMPLATE CREATION

### 1. Go to EmailJS Dashboard
→ https://dashboard.emailjs.com/admin/templates

### 2. Click "Create New Template"

### 3. Fill in these fields EXACTLY as shown:

═══════════════════════════════════════════════════════════════

## TEMPLATE SETTINGS

**Template Name:**
```
Portfolio Contact Form
```

**From Name:**
```
{{from_name}}
```

**From Email:**
```
{{from_email}}
```

**Subject:**
```
New Portfolio Message from {{from_name}}
```

**Reply To:**
```
{{from_email}}
```

**To Email:** (⚠️ Replace with YOUR email)
```
saiprasad.jnv@gmail.com
```

═══════════════════════════════════════════════════════════════

## EMAIL BODY (HTML)

Copy EVERYTHING below (including the HTML tags):

```html
<div style="font-family: Arial, sans-serif; max-width: 600px; margin: 0 auto; background: #ffffff;">
    <!-- Header -->
    <div style="background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); color: white; padding: 30px; text-align: center; border-radius: 10px 10px 0 0;">
        <h1 style="margin: 0; font-size: 28px;">📬 New Portfolio Contact</h1>
        <p style="margin: 10px 0 0 0; opacity: 0.9;">Someone reached out through your website!</p>
    </div>
    
    <!-- Content -->
    <div style="background: #f9f9f9; padding: 30px; border-radius: 0 0 10px 10px; border: 1px solid #e0e0e0; border-top: none;">
        
        <!-- Contact Info Box -->
        <div style="background: white; padding: 20px; border-radius: 8px; margin-bottom: 20px; border-left: 4px solid #667eea;">
            <h2 style="color: #667eea; margin-top: 0; font-size: 20px;">👤 Contact Information</h2>
            <table style="width: 100%; border-collapse: collapse;">
                <tr>
                    <td style="padding: 8px 0; font-weight: bold; color: #555; width: 80px;">Name:</td>
                    <td style="padding: 8px 0; color: #333;">{{from_name}}</td>
                </tr>
                <tr>
                    <td style="padding: 8px 0; font-weight: bold; color: #555;">Email:</td>
                    <td style="padding: 8px 0;">
                        <a href="mailto:{{from_email}}" style="color: #667eea; text-decoration: none;">{{from_email}}</a>
                    </td>
                </tr>
            </table>
        </div>
        
        <!-- Message Box -->
        <div style="background: white; padding: 20px; border-radius: 8px; margin-bottom: 20px; border-left: 4px solid #764ba2;">
            <h2 style="color: #764ba2; margin-top: 0; font-size: 20px;">💬 Message</h2>
            <div style="color: #333; line-height: 1.6; white-space: pre-wrap;">{{message}}</div>
        </div>
        
        <!-- Action Button -->
        <div style="text-align: center; margin-top: 30px;">
            <a href="mailto:{{from_email}}?subject=Re: Your Portfolio Message" 
               style="display: inline-block; 
                      background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); 
                      color: white; 
                      padding: 15px 40px; 
                      text-decoration: none; 
                      border-radius: 8px; 
                      font-weight: bold;
                      font-size: 16px;">
                📧 Reply to {{from_name}}
            </a>
        </div>
        
        <!-- Footer -->
        <div style="margin-top: 30px; padding-top: 20px; border-top: 1px solid #ddd; text-align: center;">
            <p style="color: #999; font-size: 12px; margin: 5px 0;">
                This email was automatically sent from your portfolio contact form
            </p>
            <p style="color: #999; font-size: 12px; margin: 5px 0;">
                <strong>Portfolio:</strong> Shiridi Sai Prasad | Software Engineer
            </p>
        </div>
    </div>
</div>
```

═══════════════════════════════════════════════════════════════

## TEMPLATE VARIABLES USED

The template uses these variables (automatically filled by your form):

- {{from_name}}  → Sender's name
- {{from_email}} → Sender's email
- {{message}}    → Message content

⚠️ DO NOT change these variable names in the template!

═══════════════════════════════════════════════════════════════

## AFTER CREATING TEMPLATE

1. Click "Save" button
2. EmailJS will show your Template ID (looks like: template_abc123)
3. COPY this Template ID
4. Save it here: _________________________________
5. You'll need this for your code!

═══════════════════════════════════════════════════════════════

## TEST YOUR TEMPLATE

Before using it in your portfolio:

1. In EmailJS dashboard, on your template page
2. Click "Test it" button
3. Fill in test values:
   ```
   from_name: John Doe
   from_email: john@example.com
   message: This is a test message from the portfolio form!
   ```
4. Click "Send Test Email"
5. Check your inbox
6. Verify the email looks good

═══════════════════════════════════════════════════════════════

## WHAT THE EMAIL WILL LOOK LIKE

📬 **Header:** Purple gradient with "New Portfolio Contact"
👤 **Contact Box:** White box with name and email (clickable)
💬 **Message Box:** White box with the full message
📧 **Reply Button:** Purple button to reply directly
📝 **Footer:** Small text with portfolio info

═══════════════════════════════════════════════════════════════

## TROUBLESHOOTING

❌ **Variables not showing?**
   → Make sure you copied the EXACT variable names
   → Check for typos: {{from_name}} not {{fromname}}

❌ **Email looks broken?**
   → Make sure you copied the ENTIRE HTML code
   → Don't modify the HTML structure

❌ **Can't save template?**
   → Make sure "To Email" field has a valid email
   → Check that all required fields are filled

═══════════════════════════════════════════════════════════════

## NEXT STEPS AFTER CREATING TEMPLATE

1. ✅ Copy Template ID
2. ✅ Get Public Key (from Account → API Keys)
3. ✅ Update advanced-portfolio.jsx with both IDs
4. ✅ Test the contact form
5. ✅ Check your email

═══════════════════════════════════════════════════════════════

🎉 **That's it!** Your contact form will be fully functional!

Time to complete: 5-7 minutes
Difficulty: Easy 🟢
