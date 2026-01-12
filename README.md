# Diet Tracker Pro 🏋️

Dashboard για tracking βάρους και compliance (D & M).

## Setup

Το dashboard τραβάει δεδομένα από Google Sheets CSV.

### Data Sheets
- **D Sheet**: Δεδομένα για D
- **M Sheet**: Δεδομένα για M

### CSV Format
```
ΗΜ/ΝΙΑ,ΗΜΕΡΑ,ΒΑΡΟΣ,ΔΙΑΙΤΑ,ΑΣΚΗΣΗ,8K,ΣΗΜΕΙΩΣΗ
12/01/26,Δευ,127.4,TRUE,FALSE,TRUE,έναρξη
```

### Αλλαγή Start/Target
Επεξεργασία `index.html`, γραμμές 268-271:
```javascript
let CONFIG = {
    D: { start: 127.4, target: 110 },
    M: { start: 65.3, target: 58 }
};
```

## Features
- 📊 Weight tracking με 7-day moving average
- 🔥 Streak counter
- 📈 Progress bars & ETA
- 📅 Consistency heatmap
- ⚖️ D vs M comparison
- 🏆 Badges & achievements
- Auto-refresh κάθε 5 λεπτά
