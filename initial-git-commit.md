# Configure git (if not already done globally)
git config user.name "BIWizzard"
git config user.email "ken@kmghub.com"  # Replace with your email

# Set main as default branch
git branch -M main

# Stage all files
git add .

# Initial commit
git commit -m "Initial project structure for Power BI Best Practices Guide

- Created 7 category folders with 35 topic placeholders
- Added README and build documentation
- Set up assets and templates folders
- Ready for content development"

# Push to GitHub
git push -u origin main