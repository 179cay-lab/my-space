# My Space Mini - PWA Todo + Expense Tracker

A lightweight, privacy-focused web app for managing todo tasks and tracking expenses with photos.

## 🚀 Features

### Todo Management
- ✅ Add/complete/delete todos
- 📊 Track total todos and completed count
- 🕐 Timestamps for each task
- 🔐 PIN-protected access

### Expense Tracker with Camera
- 📸 Capture or upload photos of receipts
- 🖼️ Image preview before saving
- 💰 Automatic amount suggestions (1K, 10K, 100K, 1M)
- 📁 Categorized expenses (Ăn uống, Di chuyển, Giải trí, etc.)
- 🗑️ Delete expenses with storage savings shown
- 📱 Automatic image compression for optimal storage

### Statistics Dashboard
- 📊 Total monthly spending + daily average
- 📈 Today's expenses + this week's total
- 💳 Category breakdown with percentages
- 📅 Last 7 days chart visualization
- 🗓️ Daily spending trends

### Smart Features
- 🧹 Auto-cleanup: Ask to delete old month's images when entering new month
- 💾 Storage optimization: Shows KB saved after cleanup
- 🔄 Monthly reconciliation: Automatic expense summary by category
- 💾 Local storage: Everything saved on your device (no server)
- 🔒 PIN protection: 4-digit PIN (default: 6089)
- 📱 PWA: Install as app on home screen

## 🔐 Default PIN
- PIN: **6089**
- ⚠️ Change this immediately for security!

## 💻 How to Use

1. **Enter PIN** - Use 4-digit PIN to access
2. **Choose Tab**:
   - **Todo**: Manage your task list
   - **Chi tiêu**: Track expenses with photos
   - **Thống kê**: View analytics and charts

### Adding Expense
1. Click 📸 to capture/upload photo
2. Preview will show after selection
3. Choose category
4. Enter product name
5. Enter price (or select suggested amount)
6. Click "Lưu chi tiêu"

### Managing Storage
- Expenses older than current month are automatically identified
- When entering new month, you'll be asked to delete old images
- See storage size in KB on Expense tab
- Manual cleanup: Click "Dọn ảnh tháng cũ"

### Viewing Statistics
- Go to "Thống kê" tab
- See total spending, daily average, and daily trends
- Category breakdown shows % of spending per category
- Only shows current month's data

## 📦 Installation

### Web Browser
1. Open index.html in any modern browser
2. Save PIN code somewhere safe
3. Click "Add to Home Screen" to install as PWA

### Deploy to GitHub Pages
```bash
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR_USERNAME/my-space.git
git push -u origin main
```
Then enable GitHub Pages in repository settings.

## 📱 PWA Support
- Works offline after first visit
- Install as app on mobile (add to home screen)
- Responds like native app
- Service Worker caching for fast loading

## 🔒 Privacy & Security
- ✅ All data stored locally on your device
- ✅ No server uploads
- ✅ No tracking
- ✅ PIN-protected
- ✅ Delete everything anytime

## 🛠️ Technical Details
- Vanilla JavaScript (no dependencies)
- LocalStorage for persistence
- Canvas for image compression
- PWA with Service Worker
- Responsive design (mobile-first)

## ⚠️ Important Notes
1. **Change the PIN**: Default is 6089 - change it for security
2. **Browser Storage Limits**: Most browsers support 5-50MB localStorage
3. **Image Storage**: Images are heavily compressed to save space
4. **Backup**: Consider exporting your data periodically
5. **Cleanup**: Old month images are removed to optimize storage

## 📊 Data Export (Manual)
Open browser DevTools → Console and run:
```javascript
console.log(JSON.stringify(DB, null, 2));
```
Copy and save the JSON output.

## 🐛 Troubleshooting

### Forgot PIN?
- Clear localStorage: Settings → Clear browsing data → Cookies & site data
- Restart and use default PIN: 6089

### Storage Full?
- Click "Dọn ảnh tháng cũ" to delete previous month's images
- Check remaining storage in Expense tab

### Image Not Showing
- Clear cache and reload
- Re-upload the image
- Try smaller file size

## 📝 License
Free to use and modify for personal use.

---

**Version**: 2.0 (Enhanced)
**Last Updated**: 2024
**Created for**: Privacy-focused expense tracking
