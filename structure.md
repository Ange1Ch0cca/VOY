voy/                                           # 📦 PROYECTO RAÍZ
│
├── public/                                    # 🌐 ÚNICA CARPETA PÚBLICA
│   ├── index.php                              # Front Controller
│   ├── .htaccess
│   │
│   ├── assets/
│   │   ├── css/
│   │   ├── js/
│   │   ├── images/
│   │   ├── icons/
│   │   ├── fonts/
│   │   └── audio/
│   │
│   ├── uploads/
│   │   ├── profiles/
│   │   ├── vehicles/
│   │   └── temp/
│   │
│   └── maps/
│
│
├── app/
│
│   ├── Core/
│   │   ├── Application.php
│   │   ├── Router.php
│   │   ├── Controller.php
│   │   ├── Database.php
│   │   ├── Request.php
│   │   ├── Response.php
│   │   ├── Validator.php
│   │   ├── Session.php
│   │   ├── Auth.php
│   │   ├── Helpers.php
│   │   └── ExceptionHandler.php
│   │
│   │
│   ├── Controllers/
│   │
│   │   ├── AuthController.php
│   │   ├── UserController.php
│   │   ├── DriverController.php
│   │   ├── PassengerController.php
│   │   ├── TripController.php
│   │   ├── LocationController.php
│   │   ├── WalletController.php
│   │   ├── RechargeController.php
│   │   ├── SubscriptionController.php
│   │   ├── NotificationController.php
│   │   │
│   │   └── Admin/
│   │       ├── DashboardController.php
│   │       ├── AdminUserController.php
│   │       ├── AdminDriverController.php
│   │       ├── AdminPassengerController.php
│   │       ├── AdminTripController.php
│   │       ├── AdminRechargeController.php
│   │       ├── AdminSubscriptionController.php
│   │       ├── AdminWalletController.php
│   │       ├── AdminSystemController.php
│   │       └── AdminReportController.php
│   │
│   │
│   ├── Models/
│   │   ├── User.php
│   │   ├── Driver.php
│   │   ├── Passenger.php
│   │   ├── Vehicle.php
│   │   ├── Trip.php
│   │   ├── Wallet.php
│   │   ├── Recharge.php
│   │   ├── Subscription.php
│   │   ├── Location.php
│   │   ├── Notification.php
│   │   ├── SystemSetting.php
│   │   └── AuditLog.php
│   │
│   │
│   ├── Services/
│   │   ├── AuthService.php
│   │   ├── TripService.php
│   │   ├── LocationService.php
│   │   ├── WalletService.php
│   │   ├── RechargeService.php
│   │   ├── SubscriptionService.php
│   │   ├── CommissionService.php
│   │   ├── NotificationService.php
│   │   ├── SystemModeService.php
│   │   ├── ReportService.php
│   │   └── AuditService.php
│   │
│   │
│   ├── Repositories/
│   │   ├── UserRepository.php
│   │   ├── DriverRepository.php
│   │   ├── PassengerRepository.php
│   │   ├── VehicleRepository.php
│   │   ├── TripRepository.php
│   │   ├── WalletRepository.php
│   │   ├── RechargeRepository.php
│   │   ├── SubscriptionRepository.php
│   │   ├── NotificationRepository.php
│   │   ├── SystemRepository.php
│   │   └── AuditRepository.php
│   │
│   │
│   ├── Middlewares/
│   │   ├── AuthMiddleware.php
│   │   ├── GuestMiddleware.php
│   │   ├── RoleMiddleware.php
│   │   ├── BalanceMiddleware.php
│   │   ├── SubscriptionMiddleware.php
│   │   ├── SystemModeMiddleware.php
│   │   ├── CsrfMiddleware.php
│   │   └── RateLimitMiddleware.php
│   │
│   │
│   ├── Views/
│   │   ├── layouts/
│   │   ├── auth/
│   │   ├── driver/
│   │   ├── passenger/
│   │   ├── admin/
│   │   ├── errors/
│   │   └── components/
│   │
│   │
│   ├── Interfaces/
│   │   ├── RepositoryInterface.php
│   │   ├── NotificationInterface.php
│   │   └── LocationProviderInterface.php
│   │
│   │
│   ├── Enums/
│   │   ├── UserRole.php
│   │   ├── DriverStatus.php
│   │   ├── TripStatus.php
│   │   ├── RechargeStatus.php
│   │   ├── SubscriptionStatus.php
│   │   └── WalletType.php
│   │
│   │
│   ├── Exceptions/
│   │   ├── AuthenticationException.php
│   │   ├── AuthorizationException.php
│   │   ├── ValidationException.php
│   │   ├── WalletException.php
│   │   └── TripException.php
│   │
│   │
│   └── Integrations/
│       ├── GoogleMaps/
│       ├── Firebase/
│       └── WhatsApp/
│
│
├── realtime/
│   ├── server.php
│   ├── Tracker.php
│   ├── LocationStream.php
│   │
│   └── Events/
│       ├── DriverMoved.php
│       ├── TripRequested.php
│       ├── TripAccepted.php
│       ├── TripStarted.php
│       ├── TripFinished.php
│       └── DriverDisconnected.php
│
│
├── admin-panel/
│   ├── index.php
│   ├── assets/
│   ├── js/
│   └── views/
│
│
├── config/
│   ├── app.php
│   ├── database.php
│   ├── wallet.php
│   ├── maps.php
│   ├── realtime.php
│   └── system.php
│
│
├── routes/
│   ├── web.php
│   ├── api.php
│   ├── admin.php
│   └── realtime.php
│
│
├── database/
│   ├── migrations/
│   │   ├── users.sql
│   │   ├── drivers.sql
│   │   ├── passengers.sql
│   │   ├── vehicles.sql
│   │   ├── trips.sql
│   │   ├── wallets.sql
│   │   ├── recharges.sql
│   │   ├── subscriptions.sql
│   │   ├── notifications.sql
│   │   ├── system_settings.sql
│   │   └── audit_logs.sql
│   │
│   └── seeders/
│
│
├── storage/
│   ├── cache/
│   ├── logs/
│   ├── sessions/
│   ├── receipts/
│   │   ├── yape/
│   │   └── efectivo/
│   │
│   └── backups/
│
│
├── bootstrap/
│   ├── app.php
│   └── autoload.php
│
│
├── .env
├── .env.example
├── composer.json
├── README.md
├── LICENSE
└── .gitignore