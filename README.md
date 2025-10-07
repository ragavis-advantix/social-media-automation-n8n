
# Smart Social Media Automation

An automated workflow to generate, approve, and post social media content daily.
The system integrates with Google Sheets for topic extraction, uses AI to create captions and images, handles client approvals via Gmail, uploads images to Cloudinary, and publishes content to Instagram, LinkedIn, and Twitter/X.

---

## 📖 Features

* ⏰ **Daily Scheduling** – Automatically triggers workflow at set times (e.g., 9 AM & 3 PM)
* 📊 **Google Sheets Integration** – Reads new media post links and topics
* 🤖 **AI Content Generation** – Uses Google Gemini AI for captions and images
* 📂 **Image Hosting** – Uploads AI-generated images to Cloudinary
* 📧 **Approval Workflow** – Sends content for client approval via Gmail
* 🌐 **Multi-platform Posting** – Publishes content to Instagram, LinkedIn, and Twitter/X
* 🔔 **Client Notifications** – Sends confirmation emails with social media links after posting

---

## 🛠️ Tech Stack

* **n8n** – Workflow automation engine
* **Google Gemini AI** – For generating captions and images
* **Google Sheets API** – For fetching topics and links
* **Gmail API** – For approval workflow and notifications
* **Cloudinary** – Image hosting
* **Facebook Graph API** – Instagram publishing
* **Twitter/X API** – Posting media and captions
* **LinkedIn API** – Publishing posts

---

## ⚙️ Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/ragavis-advantix/social-media-automation.git
cd social-media-automation
```

### 2. Import Workflow into n8n

* Open the n8n dashboard
* Import `workflow.json`
* Configure credentials for:

  * Google Sheets
  * Gmail
  * Cloudinary
  * Facebook Graph API (Instagram)
  * Twitter/X API
  * LinkedIn

### 3. Configure Workflow Nodes

* Update Google Sheet ID and columns
* Adjust wait node timings if needed
* Verify AI models and prompts for captions & images

### 4. Verify Workflow

* Test with sample rows in Google Sheets
* Ensure Gmail approval emails are sent and responded to
* Check that images are uploaded to Cloudinary
* Confirm posts appear correctly on Instagram, LinkedIn, and Twitter/X

---

## 📝 Development Notes

* **Customization**:

  * Modify AI prompts for different content styles
  * Adjust social media posting schedules or add new platforms

* **Scaling**:

  * Add Slack or Teams notifications
  * Store images on S3 or alternative hosting

* **Testing**:

  * Use test Google Sheet rows for dry-run tests
  * Logs in n8n help debug workflow failures

---

## 👨‍💻 Author

**Ragavi**

📧 Email: [ragavis@advantixagi.com](mailto:ragavis@advantixagi.com)


Do you want me to do that?
