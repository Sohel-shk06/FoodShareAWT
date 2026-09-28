FoodShareAWT/
│
├── src/
│   │
│   ├── main/
│   │   └── Main.java                     // App entry point (AWT EventQueue runner)
│   │
│   ├── config/
│   │   ├── DBConnection.java             // JDBC Connection Manager
│   │   └── DatabaseInitializer.java      // Tables auto-creator
│   │
│   ├── model/                            // POJO Entities
│   │   ├── User.java                     // User aur NGO details
│   │   ├── Donation.java                 // Food donation items
│   │   └── FoodRequest.java              // NGO/User requests
│   │
│   ├── dao/                              // Database Queries (SQL Logic)
│   │   ├── UserDAO.java                  // Login aur registration queries
│   │   ├── DonationDAO.java              // Food insert aur fetch queries
│   │   └── RequestDAO.java               // Status update (Accept/Reject)
│   │
│   ├── ui/                               // Presentation Layer (Pure java.awt.*)
│   │   ├── MainFrame.java                // java.awt.Frame (WindowListener + CardLayout)
│   │   │
│   │   ├── components/                   // AWT Custom Widgets (Missing controls ka solution)
│   │   │   ├── CustomTablePanel.java     // JTable ki jagah custom rows & scrollable list
│   │   │   ├── CustomCardPanel.java      // Dashboard ke 2x2 clickable cards
│   │   │   ├── CustomNavButton.java      // Sidebar navigation buttons
│   │   │   └── StatusBadge.java          // Pending / Accepted / Completed chips
│   │   │
│   │   └── panels/                       // Screens (Sab java.awt.Panel extend karenge)
│   │       ├── LoginPanel.java           // Screen 1: CheckboxGroup (Radio) + Form
│   │       ├── HomePanel.java            // Screen 2: Welcome banner + 4 cards
│   │       ├── DonatePanel.java          // Screen 3: Label, TextField, Choice dropdown
│   │       ├── AvailableFoodPanel.java   // Screen 4: Search + CustomTablePanel
│   │       ├── ActivityPanel.java        // Screen 5: Stats + History Table
│   │       ├── ProfilePanel.java         // Screen 6: User details & Settings
│   │       └── NgoDashboardPanel.java    // Screen 7: NGO Approval Table & Buttons
│   │
│   └── util/
│       ├── AWTConstants.java             // java.awt.Color, java.awt.Font constants
│       └── UserSession.java              // Logged-in user session state
│
└── README.md