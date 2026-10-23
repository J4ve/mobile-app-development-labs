# Graph Report - mobile-app-development-labs  (2026-10-23)

## Corpus Check
- Large corpus: 500 files · ~680,437 words. Semantic extraction will be expensive (many Claude tokens). Consider running on a subfolder.

## Summary
- 200 nodes · 300 edges · 13 communities (10 shown, 3 thin omitted)
- Extraction: 93% EXTRACTED · 7% INFERRED · 0% AMBIGUOUS · INFERRED: 22 edges (avg confidence: 0.89)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- WeatherApp
- CCCS 106 Projects README
- app_logic.py
- Watchlist
- .__init__()
- WeatherCache
- WeatherService
- Weather Application (Flet +
- my-flet-app/src/main.py
- connect_db()
- contact-book-app
- my-flet-app
- userlogin

## God Nodes (most connected - your core abstractions)
1. `WeatherApp` - 34 edges
2. `WeatherService` - 15 edges
3. `Watchlist` - 14 edges
4. `WeatherCache` - 13 edges
5. `CCCS 106 Projects README` - 10 edges
6. `Weather Application (Flet + OpenWeatherMap)` - 10 edges
7. `WeatherServiceError` - 9 edges
8. `display_contacts()` - 8 edges
9. `Flet 0.28.3 GUI Framework` - 8 edges
10. `Config` - 7 edges

## Surprising Connections (you probably didn't know these)
- `mod6_labs requirements.txt (pip freeze, UTF-16)` --semantically_similar_to--> `CCCS 106 root requirements.txt (pip freeze, UTF-16)`  [INFERRED] [semantically similar]
  mod6_labs/requirements.txt → requirements.txt
- `WeatherCache` --implements--> `Weather Data Caching and Offline Mode`  [INFERRED]
  mod6_labs/cache.py → mod6_labs/README.md
- `Watchlist` --implements--> `Multiple Cities Comparison with Watchlist (watchlist.json)`  [INFERRED]
  mod6_labs/watchlist.py → mod6_labs/README.md
- `CCCS 106 Projects README` --references--> `CCCS 106 root requirements.txt (pip freeze, UTF-16)`  [INFERRED]
  README.md → requirements.txt
- `Weather Application (Flet + OpenWeatherMap)` --references--> `Flet 0.28.3 GUI Framework`  [EXTRACTED]
  mod6_labs/README.md → README.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Identical Flet project-template READMEs (uv/poetry run + flet build targets)** — mobile_app_development_labs_week3_labs_readme, mobile_app_development_labs_week4_labs_contact_book_app_readme, mobile_app_development_labs_sample_apk_build_my_flet_app_readme [INFERRED 0.95]

## Communities (13 total, 3 thin omitted)

### Community 0 - "WeatherApp"
Cohesion: 0.08
Nodes (20): Update comparison button visibility and text., Toggle between single weather and comparison view., Return to single city weather view., Format timestamp to readable 'last updated' string., Get weather for current location., Main Weather Application class., Toggle between current weather and forecast view., Helper to fade out forecast and show weather. (+12 more)

### Community 1 - "CCCS 106 Projects README"
Cohesion: 0.12
Nodes (21): Weather Application README (Module 6 Lab), mod6_labs requirements.txt (pip freeze, UTF-16), PyInstaller 6.16.0 (desktop executable packaging), CCCS 106 Projects README, cccs106_env Virtual Environment, CCCS 106 Application Development and Emerging Technologies (course, AY 2025-2026), Flet 0.28.3 GUI Framework, Jave Atanacio Bacsain (author, BSCS-3A, ID 231003016) (+13 more)

### Community 2 - "app_logic.py"
Cohesion: 0.13
Nodes (23): add_contact(), delete_contact(), display_contacts(), open_edit_dialog(), Opens a dialog to edit a contact's details., Fetches and displays all contacts in the ListView., Adds a new contact and refreshes the list., Deletes a contact and refreshes the list. (+15 more)

### Community 3 - "Watchlist"
Cohesion: 0.12
Nodes (12): Search History with Persistent Storage (search_history.json), Multiple Cities Comparison with Watchlist (watchlist.json), Manage a list of cities for weather comparison., Initialize the watchlist manager. Args: filename: Name of the file to store…, Load watchlist from file. Returns: List of city names in the watchlist, Save current watchlist to file., Add a city to the watchlist. Args: city: Name of the city to add Returns: True…, Remove a city from the watchlist. Args: city: Name of the city to remove… (+4 more)

### Community 4 - ".__init__()"
Cohesion: 0.11
Nodes (10): Button, Dropdown, Page, Build button that uses the user's location, Configure page settings., Build the user interface., Handle search button click or enter key press., Load search history from file. (+2 more)

### Community 5 - "WeatherCache"
Cohesion: 0.11
Nodes (9): Cache manager for weather data with expiration logic., Cache forecast data for a city. Args: city: Name of the city data: Forecast…, Get the timestamp of cached forecast data. Args: city: Name of the city…, Initialize the cache manager. Args: cache_dir: Directory to store cache files…, Get cached weather data for a city. Args: city: Name of the city Returns:…, Cache weather data for a city. Args: city: Name of the city data: Weather data…, Get the timestamp of cached data. Args: city: Name of the city Returns:…, Get cached forecast data for a city. Args: city: Name of the city Returns:… (+1 more)

### Community 6 - "WeatherService"
Cohesion: 0.18
Nodes (14): Test handling of invalid city., Test handling of empty city name., Test fetching weather for a valid city., run_tests(), test_empty_city(), test_invalid_city(), test_valid_city(), Exception (+6 more)

### Community 7 - "Weather Application (Flet +"
Cohesion: 0.22
Nodes (10): Config, Application configuration., Validate that required configuration is present., main(), Weather Data Caching and Offline Mode, 5-Day Weather Forecast with Tabbed Interface, Current Location Weather via IP Geolocation, ipgeolocation.io API (+2 more)

### Community 8 - "my-flet-app/src/main.py"
Cohesion: 0.22
Nodes (6): Toggle between light and dark theme., main(), Page, Simple Task Manager App - Flet Demo A cross-platform task management…, Task, TaskManagerApp

### Community 9 - "connect_db()"
Cohesion: 0.40
Nodes (4): Userlogin App README (Flet project template), connect_db(), main(), Page

## Knowledge Gaps
- **5 isolated node(s):** `my-flet-app`, `userlogin`, `contact-book-app`, `ipgeolocation.io API`, `GitHub repo J4ve/cccs106-projects`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 78 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **3 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `WeatherApp` connect `WeatherApp` to `Watchlist`, `.__init__()`, `WeatherService`, `Weather Application (Flet +`, `my-flet-app/src/main.py`?**
  _High betweenness centrality (0.497) - this node is a cross-community bridge._
- **Why does `Weather Application (Flet + OpenWeatherMap)` connect `Weather Application (Flet +` to `CCCS 106 Projects README`, `Watchlist`?**
  _High betweenness centrality (0.402) - this node is a cross-community bridge._
- **Why does `Flet 0.28.3 GUI Framework` connect `CCCS 106 Projects README` to `Weather Application (Flet +`?**
  _High betweenness centrality (0.387) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `WeatherApp` (e.g. with `Config` and `Watchlist`) actually correct?**
  _`WeatherApp` has 3 INFERRED edges - model-reasoned connections that need verification._
- **Are the 3 inferred relationships involving `WeatherService` (e.g. with `WeatherApp` and `WeatherCache`) actually correct?**
  _`WeatherService` has 3 INFERRED edges - model-reasoned connections that need verification._
- **Are the 2 inferred relationships involving `Watchlist` (e.g. with `WeatherApp` and `Multiple Cities Comparison with Watchlist (watchlist.json)`) actually correct?**
  _`Watchlist` has 2 INFERRED edges - model-reasoned connections that need verification._
- **Are the 2 inferred relationships involving `WeatherCache` (e.g. with `Weather Data Caching and Offline Mode` and `WeatherService`) actually correct?**
  _`WeatherCache` has 2 INFERRED edges - model-reasoned connections that need verification._