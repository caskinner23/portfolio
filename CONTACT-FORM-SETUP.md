# Contact Form Setup Instructions

Your contact form is built and ready! You just need to connect it to Formspree so emails get sent to you.

## Step 1: Sign Up for Formspree (Free)

1. Go to [formspree.io](https://formspree.io)
2. Click "Get Started" (it's free!)
3. Sign up with your email (or GitHub/Google)
4. Verify your email address

## Step 2: Create Your Form

1. Once logged in, click **"+ New Form"**
2. Give it a name: "Portfolio Contact Form"
3. Click "Create Form"
4. You'll see your **Form ID** - it looks like: `xyzabc123`

## Step 3: Update Your Contact Page

1. Open `/Users/caskinner/Documents/cassandra-portfolio-website/contact.html`
2. Find this line (around line 127):
   ```html
   <form id="contact-form" class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
3. Replace `YOUR_FORM_ID` with your actual Formspree form ID
4. Find this line (around line 165):
   ```html
   <input type="hidden" name="_next" value="https://your-username.github.io/contact.html?success=true">
   ```
5. Replace `your-username.github.io` with your actual GitHub Pages URL (we'll set this up next)
6. Save the file

## Step 4: Configure Formspree Settings (Optional but Recommended)

In your Formspree dashboard, you can:

### Email Settings:
- **Reply-To Address:** Set to the submitter's email so you can reply directly
- **Email Notifications:** You'll get emails at the address you signed up with
- **Subject Line:** Already set to "New contact form submission from portfolio"

### Spam Protection:
- **reCAPTCHA:** Enable this to prevent spam (Formspree has built-in protection)
- **Honeypot:** Already enabled in your form (the hidden `_gotcha` field)

### Autoresponder (Optional):
- Set up an automatic "Thanks for reaching out!" email to people who submit

## How It Works

1. **Visitor fills out form** on your contact page
2. **Formspree receives** the submission
3. **You get an email** with all the form data:
   - Name
   - Email
   - Company
   - Reason for contact
   - Message
4. **Visitor sees success message** and can choose to email/LinkedIn directly too
5. **You reply** directly from your email inbox

## Free Tier Limits

- **50 submissions/month** (plenty for a portfolio)
- **Unlimited forms**
- **Spam filtering included**

If you get more than 50 submissions, you can upgrade for $10/month.

## Testing Your Form

Once you've updated the Form ID:

1. Save the contact.html file
2. Open it in your browser
3. Fill out the form with test data
4. Click "Send Message"
5. You should get redirected to a success message
6. Check your email - you should receive the submission!

## Troubleshooting

**Form doesn't submit:**
- Check that you replaced `YOUR_FORM_ID` with your actual Formspree ID
- Make sure you're online

**Not receiving emails:**
- Check your spam folder
- Verify your email in Formspree dashboard
- Check Formspree dashboard for submissions

**Success message not showing:**
- Make sure the `_next` URL matches your deployed site URL
- For local testing, it might not redirect properly - that's normal

---

## Alternative: Direct Email Link

If you prefer not to use a form, I can change the contact page to just have a large "Email Me" button that opens their email client. Let me know!
