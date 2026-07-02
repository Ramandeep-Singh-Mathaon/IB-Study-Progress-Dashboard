# IB Study Progress Dashboard

A Power BI dashboard that tracks my daily IB study time across HL and SL subjects, so I can see — instead of guess — where my time actually goes.

## Why I built this

Partway through the IB Diploma I noticed I *felt* like I was studying Physics a lot and Computer Science barely at all, but I had no data to check that against. This project replaced the feeling with a log.

## How it works

1. Study sessions are logged manually in `Study_Time_Tracker_IB.xlsx` (subject, date, duration).
2. `Progress.pbix` reads that spreadsheet and builds three views: an overview of the last 7 days, an HL breakdown, and an SL breakdown.
3. The dashboard is refreshed by re-opening the `.pbix` file in Power BI Desktop after updating the spreadsheet.

## Dashboard preview

| Overview | HL Subjects | SL Subjects |
|---|---|---|
| ![Overview](Overview.png) | ![HL](HL.png) | ![SL](SL.png) |

## What it's for

The goal isn't a one-time report — it's a habit of checking assumptions against real data instead of going by feel. I'm still building up logged history, so I'm not drawing firm conclusions yet; the dashboard is the mechanism for catching real patterns as the log grows, not a finished analysis.

## Limitations (read this before trusting the numbers)

This is self-reported, manually-logged data, not sensor- or app-tracked time. That means it's subject to the usual biases of self-tracking: sessions may be rounded up, short sessions may go unlogged entirely, and "study time" isn't the same as focused time. Treat the dashboard as a directional signal, not a precise measurement.

## Files

| File | Purpose |
|---|---|
| `Progress.pbix` | Power BI dashboard (open in Power BI Desktop) |
| `Study_Time_Tracker_IB.xlsx` | Underlying logged data |
| `Dashboard_Background.png`, `Overview.png`, `HL.png`, `SL.png` | Dashboard background and preview screenshots |

## Tools used

Power BI · Excel · Git/GitHub

## Where this is going

This dashboard is the first version of an ongoing project. The next iteration moves the analysis from Power BI into a proper Python/ML pipeline that predicts which subjects need more attention — details to follow in a dedicated repo once it's built.

## License

MIT — see [`LICENSE`](LICENSE).

## Author

Ramandeep Singh Mathaon · [LinkedIn](https://www.linkedin.com/in/ramandeep-singh-mathaon-b42795386)
