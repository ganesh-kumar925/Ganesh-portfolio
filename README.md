# 🎮 3D Gaming Portfolio

A modern, cyberpunk-themed portfolio with 3D animations and gaming aesthetics.

## 🚀 Features

- ✨ 3D rotating cube loading screen
- 🎯 Separate pages for About, Skills, Projects, Contact
- 💫 Particle star background
- 🔮 3D card hover effects
- ⚡ Glitch text animations
- 🌈 Cyberpunk neon theme (cyan + magenta)

## 📦 Deployment

This portfolio automatically deploys to AWS S3 using GitHub Actions.

### Setup Instructions:

1. **Create an S3 Bucket:**
   - Go to AWS S3 Console
   - Create a new bucket (e.g., `ganesh-portfolio`)
   - Enable "Static website hosting"
   - Set index document to `index.html`
   - Make bucket public (update bucket policy)

2. **Create IAM User:**
   - Go to AWS IAM Console
   - Create a new user with programmatic access
   - Attach policy: `AmazonS3FullAccess`
   - Save the Access Key ID and Secret Access Key

3. **Add GitHub Secrets:**
   - Go to your GitHub repository
   - Settings → Secrets and variables → Actions
   - Add these secrets:
     - `AWS_ACCESS_KEY_ID` - Your AWS access key
     - `AWS_SECRET_ACCESS_KEY` - Your AWS secret key
     - `S3_BUCKET_NAME` - Your S3 bucket name (e.g., ganesh-portfolio)
     - `CLOUDFRONT_DISTRIBUTION_ID` - (Optional) If using CloudFront

4. **Push to GitHub:**
   ```bash
   git add .
   git commit -m "Add GitHub Actions deployment"
   git push origin main
   ```

5. **Access Your Site:**
   - Your portfolio will be live at: `http://your-bucket-name.s3-website-us-east-1.amazonaws.com`

## 🛠️ Technologies

- HTML5
- CSS3 (3D Transforms, Animations)
- GitHub Actions
- AWS S3

## 📧 Contact

- Email: pathakotaganeshkr3@gmail.com
- Phone: 9182046096

---

© 2025 Ganesh Kumar. All Rights Reserved.
