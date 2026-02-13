# ⚡ Nexus Admin Dashboard | REST API Integration - Task 16

**A professional, dual-purpose admin interface aggregating data from public REST APIs using Vanilla JavaScript.**

### 🔴 **Live Demo:** [Click Here to View](https://sharanx77.github.io/task_16.elevateslabs/)

---

## 🚀 About The Project

**"Nexus Admin Dashboard"** was developed for the **Elevate Labs Web Development Internship (Task 16)**. This project demonstrates the ability to build a data-driven Frontend application that consumes live data from external servers. The dashboard interacts with two distinct public APIs to simulate a real-world enterprise environment, handling asynchronous data fetching, error management, and efficient DOM updates directly in the browser.

### 🎯 Key Features
* **Dual-API Integration:** Seamlessly aggregates data from **FakeStore API** (E-Commerce Inventory) and **CoinLore API** (Real-time Crypto Market).
* **Strict Lazy Loading:** Implements smart state management (`isLoaded` flags) to ensure APIs are only called when the user explicitly clicks a tab, reducing network bandwidth and improving performance.
* **Live Search & Filtering:** Features a real-time search bar for the Store Inventory, filtering product arrays instantly on the client side without reloading the page.
* **Dynamic DOM Rendering:** Utilizes JavaScript ES6 Template Literals and `.map()` methods to inject HTML content programmatically.
* **Visual Data Feedback:** Includes conditional formatting (Green/Red indicators) for cryptocurrency price changes to represent market trends visually.
* **Robust Error Handling:** Implements `try...catch` blocks to gracefully handle network failures, ensuring the application UI remains stable even if an API is temporarily unreachable.

---

## 🧰 Tech Stack

* **HTML5:** Semantic structure with a sidebar layout and tabbed content sections.
* **CSS3:**
    * **Flexbox & CSS Grid:** For responsive product card layouts and sidebar navigation.
    * **CSS Variables:** For consistent color theming (Dark Sidebar, Light Content).
    * **Keyframe Animations:** Smooth fade-in effects when switching tabs.
* **JavaScript (ES6+):**
    * **Fetch API:** Asynchronous data retrieval using `async` / `await`.
    * **State Management:** Local boolean flags to track data loading status.
    * **Array Methods:** Extensive use of `.filter()`, `.map()`, and `.slice()` for data manipulation.
* **External APIs:**
    * [Fake Store API](https://fakestoreapi.com/) (Product Data)
    * [CoinLore API](https://www.coinlore.com/cryptocurrency-data-api) (Crypto Market Data)

---

## 🛠️ Technical Implementation Details
This project fulfills the specific requirements for Task 16:

* **Asynchronous Data Flow:** The application uses `async/await` patterns to ensure the UI remains responsive while waiting for server responses.
* **Single-Page Logic:** Although not a full router, the application functions as a Single-Page Interface. Clicking sidebar items toggles visibility classes (`display: none/block`) rather than reloading the page, preserving the application state.
* **Optimized Fetching:** The "Traffic Jam" issue common in single-page apps is solved by isolating fetch requests. The Crypto data is never requested until the user actually navigates to that tab.
```
/Task_16_REST_API_Dashboard
│
├── index.html        # Main Dashboard (Contains HTML, CSS, and JS logic)
└── README.md         # Project Documentation
```
## 🔮 Future Roadmap
* ✅ **Phase 1:** (Completed) Core dashboard layout, API fetching, and filtering logic.
* 🔄 **Phase 2:** Add a **"Detail View" Modal** that opens when clicking on a product card to show the full description.
* 🔄 **Phase 3:** Implement **Chart.js** to visualize the Bitcoin price history in a line graph.
* 🔄 **Phase 4:** Add a "Sort by Price" button to toggle between Low-to-High and High-to-Low.

---

## 👨‍💻 Author
**B Sharana Basava**
*Electronics and Communication Engineering Student*

* **LinkedIn:** [B Sharana Basava](https://www.linkedin.com/in/b-sharanabasava-b4313a325)
* **GitHub:** [Sharanx77](https://github.com/Sharanx77)
* **Email:** [b.sharanabasava2006@gmail.com](mailto:b.sharanabasava2006@gmail.com)

---

## 🙌 Acknowledgments
* **Elevate Labs** for the challenge to integrate REST APIs into frontend applications.
* **CoinLore & FakeStoreAPI** for providing free, high-quality public data for developers.
* **Gemini AI** for assistance with optimizing fetch logic and state management.
