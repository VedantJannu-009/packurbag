# Tour Buddy

Tour Buddy is a travel support app designed to enhance your travel experience with various features including category-based to-do task lists, currency converter, calculator, language translation, and emergency SOS.

## Features

- **Category-based To-Do Task List**: Organize your tasks by categories such as sightseeing, dining, accommodation, etc., to stay organized during your travels.
- **Currency Converter**: Easily convert currencies to help you manage your expenses and budget effectively in different countries.
- **Calculator**: Perform quick calculations while on the go, whether it's budgeting or splitting bills with friends.
- **Language Translation**: Overcome language barriers with built-in translation features, helping you communicate effectively in foreign countries.
- **Emergency SOS**: Access emergency assistance quickly with the SOS feature, providing peace of mind during your travels.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Om-jannu/packurbag.git
   ```

2. Navigate into the project directory:

   ```bash
   cd packurbag
   ```

3. Install dependencies for flutter:
   ```bash
   flutter pub get
   ```
4. Install dependencies for server:

   ```bash
   cd server
   ```

   ```bash
   npm install
   ```

## Usage

### Server Setup (Step 1.):

1. Create `.env` file inside the server diretory and add :
   (**Note: use appropriate mongo url**)

```
MONGO_URL="mongodb+srv://<username>:<password>@beyondthebasics.abcde.mongodb.net/test"
PORT=5000
```

1. Run server:

```bash
npm run dev
```

Here's a guide for setting up Ngrok and starting port forwarding:

### Ngrok Setup & Installation  (Step 2):

1. **Download Ngrok**:

   - Go to the [Ngrok website](https://ngrok.com/) and sign up for an account if you haven't already.
   - Download the Ngrok executable suitable for your operating system.
   
2. **Start Port Forwarding**:
   - Open a terminal or command prompt window.
   - To start port forwarding, run the following command:
     ```
     ngrok http 5000
     ```
     This command starts forwarding traffic from Ngrok's randomly generated public URL to your local server running on port 5000.
3. **Copy the public URL**.

`Note: if ngrok command doesn't work on cmd prompt, try running with admin privileges or sudo privileges`

### Flutter Setup  (Step 3.):

1. Choose an android emulator
2. Change **serverIp** in `lib/main.dart` file
```
const serverIp = "<ngrok-public-url>";
example : https://cb4f-103-xxx-xxx-122.ngrok-free.app;
```
3. Run Command
```
flutter pub get
flutter run
```

## Screenshots

##### 1. QuickActions, Login & Register

<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/7020f412-73e0-44f6-9ca9-8082a857aa15" />


##### 2. Home & AddTodo

<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/a3ad5906-f431-400b-8091-cde23dff970a" />


##### 3. Category, Todolist & Translation

<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/b75d54d0-e022-46ac-8331-a2c0e7976025" />


##### 4. Bluetooth Screens

<img width="1920" height="1080" alt="4" src="https://github.com/user-attachments/assets/d3b0655f-0521-41f2-b8fe-e3c2534acfc1" />


##### 5. Calculator, Currency Converter & Profile

<img width="1920" height="1080" alt="5" src="https://github.com/user-attachments/assets/5e6445a7-5910-43cd-b806-3ce1373b7eda" />


##### 6. Emergency SOS Page

<img width="1920" height="1080" alt="6" src="https://github.com/user-attachments/assets/164514b7-d268-4444-b328-ad92e1c396c7" />


## Contributing

If you'd like to contribute to this project, please follow these guidelines:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature`)
6. Create a new Pull Request.
