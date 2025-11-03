# 💰 Salary Calculator

A responsive, mobile-friendly web app for calculating your take-home pay based on hours worked, pay frequency, and personal expenses. Perfect for tracking bi-weekly, weekly, or monthly paychecks with overtime calculations.

![Salary Calculator](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## ✨ Features

- **Flexible Pay Frequency**: Calculate for weekly, bi-weekly, or monthly pay periods
- **Overtime Calculations**: Automatically splits hours into standard and overtime with separate rates
- **Customizable Rates**: Set your own regular and overtime hourly rates
- **Tax Calculations**: Input your tax rate to see accurate take-home pay
- **Expense Tracking**: Add fixed monthly bills (supports expression format like `500+600+120`)
- **Net Spendable**: See how much you'll have left after bills per pay period
- **Mobile Optimized**: Touch-friendly interface with native number pad support
- **Visual Feedback**: Clear distinction between input fields (teal) and output results (grey)

## 🚀 Quick Start

### Online Usage

Simply open `index.html` in any modern web browser. No installation required!

### Local Server (Recommended)

For the best experience, serve the file using a local HTTP server:

```bash
# Using Python 3
python3 -m http.server 8000

# Then open http://localhost:8000 in your browser
```

## 📱 How to Use

1. **Set Your Rates**: Enter your regular hourly rate and overtime rate (typically 1.5x regular)
2. **Configure Tax Rate**: Input your effective tax rate percentage
3. **Choose Pay Frequency**: Select Weekly, Biweekly, or Monthly
4. **Enter Hours**: Input total hours worked in the pay period
5. **Add Expenses** (optional): Enter fixed monthly bills (e.g., `500+600+120`)
6. **View Results**: See your gross pay, breakdown, take-home, and net spendable amount

### Example Calculation

For a bi-weekly pay period:
- Regular Rate: `$65.00/hr`
- Overtime Rate: `$97.50/hr`
- Tax Rate: `27.32%`
- Standard Hours: `70` (35 hrs/week × 2 weeks)
- Total Hours Worked: `77.5`

**Results:**
- Standard: `70 hrs × $65 = $4,550`
- Overtime: `7.5 hrs × $97.50 = $731.25`
- Gross Pay: `$5,281.25`
- Take-Home (after 27.32% tax): `$3,838.47`

## 🎨 Features in Detail

### Pay Period Recommendations
The app automatically suggests standard hours based on your pay frequency:
- **Weekly**: 35 hours
- **Biweekly**: 70 hours (35 hrs/week)
- **Monthly**: 152 hours (~35 hrs/week)

You can override these recommendations to match your specific situation.

### Expense Calculator
Enter your fixed monthly bills using the `+` operator:
```
500+600+120 = $1,220/month
```
The app automatically calculates how much is deducted per pay period based on your frequency.

### Visual Design
- **Input Fields**: White background with teal border (editable)
- **Output Fields**: Grey background with inset shadow (read-only)
- **Mobile-First**: Large touch targets and native number keyboards
- **Smooth Gradient**: Calming blue gradient background

## 🛠️ Technical Details

- **Pure HTML/CSS/JavaScript**: No frameworks or dependencies
- **Responsive Design**: Works on all screen sizes
- **Real-time Updates**: Calculations update instantly as you type
- **Font Awesome Icons**: Professional dollar sign icon
- **Local Storage Ready**: Easy to extend with persistent settings

## 📂 Project Structure

```
Salary_Calc/
├── index.html          # Single-file application
└── README.md          # This file
```

## 🔧 Customization

### Changing Default Values

Edit the HTML file to modify default values:

```javascript
// Default rates (line ~150)
<input type="number" id="regularRate" value="65" ...>
<input type="number" id="overtimeRate" value="97.5" ...>
<input type="number" id="taxRate" value="27.3189" ...>
```

### Adding More Features

The code is well-structured and easy to extend:
- Add more input fields in the HTML
- Update `calculateSalary()` function for new calculations
- Add event listeners for real-time updates

## 🤝 Contributing

Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🐛 Bug Reports

Found a bug? Please open an issue with:
- Description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Browser/device information

## 💡 Future Enhancements

- [ ] Save/load multiple profiles
- [ ] Year-to-date earnings tracker
- [ ] Export calculations to PDF
- [ ] Dark mode support
- [ ] Multiple currency support
- [ ] Bonus/commission calculator
- [ ] Retirement contribution calculator

## 👤 Author

**JQH84**
- GitHub: [@JQH84](https://github.com/JQH84)

## 🙏 Acknowledgments

- Font Awesome for the icons
- The open-source community for inspiration

---

**Made with ❤️ for tracking personal finances**

*Last Updated: November 2025*
