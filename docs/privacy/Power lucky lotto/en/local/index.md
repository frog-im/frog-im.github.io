### 2-2) Local Settings and Stored Values (Stored Internally on the Device)

To provide this feature and maintain usability, some settings/data are stored **only locally** in the form of  
`SharedPreferences`, the app documents folder, or a local DB (SQLite/sqflite).

These values are not automatically transmitted to the developer's server and may be deleted together **when app data is cleared or the app is uninstalled (or depending on device policy)**.

#### (1) Country/Game Selection and Basic App Settings (`SharedPreferences`)

| Category | Key (Example) | Purpose | Storage Location | Deletion Timing |
|---|---|---|---|---|
| Initial setup completion status | `setup_done` | Determines whether the initial setup has been completed or skipped | SharedPreferences | When app data is cleared or the app is uninstalled |
| Country selection history | `selected_countries` | Stores the history of recently selected countries | Same as above | Same as above |
| Currently active country | `active_country` | Configures the game list based on the current country | Same as above | Same as above |
| Currently active game | `active_lotto_id` | Specifies the default game to display/use for statistics | Same as above | Same as above |
| Selected game list | `selected_lotto_ids` | Stores the list of games to use for statistics/search | Same as above | Same as above |
| App language setting | `app_locale_tag` | Applies a fixed app language instead of the system language | Same as above | Same as above |
| Ophiuchus mode | `enable_ophiuchus_mode` | Reflects extended mode in zodiac calculation/display | Same as above | Same as above |
| JSON editor sheet usage status | `json_editor_sheet_enabled` | Stores whether the JSON editor bottom sheet is shown | Same as above | Same as above |

#### (2) Selected seed time value (`SharedPreferences`)

| Category | Key (Example) | Purpose | Storage Location | Deletion Timing |
|---|---|---|---|---|
| Seed reference time (date/time) | `birth_datetime_iso` | Stores the seed reference time used for number generation/reports | SharedPreferences | When app data is cleared or the app is uninstalled |

- If the user does not separately choose a seed time, the app may generate and store the **current time value** to provide the feature.
- The stored value is a **date/time (ISO string)** and does not include direct identifiers such as an account, email address, or phone number.

#### (3) JSON Guide and Auxiliary UI Settings (`SharedPreferences`)

| Category | Key (Example) | Purpose | Storage Location | Deletion Timing |
|---|---|---|---|---|
| JSON guide one-time display flag | `json_guide_shown_{gameId}` | Prevents duplicate display of the JSON editing guide | SharedPreferences | When app data is cleared or the app is uninstalled |
| Slot record bottom sheet usage status | `slot_machine_bottom_sheet_enabled` | Stores whether the slot record bottom sheet is shown | Same as above | Same as above |

#### (4) Slot Machine Record/Probability Settings (`SharedPreferences`)

| Category | Key (Example) | Purpose | Storage Location | Deletion Timing |
|---|---|---|---|---|
| Current slot record existence status | `slot_machine_current_has_record` | Stores whether the current record exists | SharedPreferences | When app data is cleared or the app is uninstalled |
| Current slot result type | `slot_machine_current_outcome` | Stores success/failure/pending status | Same as above | Same as above |
| Current slot image number | `slot_machine_current_image_no` | Stores the currently displayed image state | Same as above | Same as above |
| Current accumulated failure count | `slot_machine_current_failure_count` | Stores the current consecutive failure count | Same as above | Same as above |
| Current success probability value | `slot_machine_current_success_rate_percent` | Stores the success probability linked to the current record | Same as above | Same as above |
| Last consumed record existence status | `slot_machine_last_has_record` | Stores whether the last usage record exists | Same as above | Same as above |
| Last consumed result type | `slot_machine_last_outcome` | Stores the success/failure status of the last record | Same as above | Same as above |
| Last consumed image number | `slot_machine_last_image_no` | Stores the image state of the last record | Same as above | Same as above |
| Last consumed failure count | `slot_machine_last_failure_count` | Stores the accumulated failure count of the last record | Same as above | Same as above |
| Last consumed success probability | `slot_machine_last_success_rate_percent` | Stores the success probability of the last record | Same as above | Same as above |
| Configured default success probability | `slot_machine_configured_success_rate_percent` | Stores the slot success probability adjusted by the user | Same as above | Same as above |

- The values above are local setting values used to maintain the slot UI state and display records.
- They are stored only inside the device and are not transmitted to a server.

#### (5) Temporary Storage for Number-Based Generation and AI Model (`SharedPreferences`)

| Category | Key (Example) | Purpose | Storage Location | Deletion Timing |
|---|---|---|---|---|
| Number-based checkpoint (v1) | `nb_checkpoint_v1_{gameId}` | Maintains legacy temporary saved records | SharedPreferences | When app data is cleared or the app is uninstalled |
| Number-based checkpoint (v2) | `nb_checkpoints_v2_{gameId}` | Stores a list of checkpoints for pause/resume | Same as above | Same as above |
| AI model setting by game | `ai_model_{gameId}` | Stores AI selection weights/slot settings by game | Same as above | Same as above |

- Checkpoints may include the number of attempts, recent numbers, seed-based values, saved time (UTC ISO string), and similar data.
- These are internal state values for resuming the feature and do not include direct identifiers.

#### (6) Local JSON File Storage (App Documents Folder)

- Path (example): app documents folder `/game_json/{gameId}.json`
- Content: game data (JSON) directly edited/managed by the user
- Purpose of use: local storage of game-specific data and support for statistics/search features
- Deletion: generally deleted together when app data is cleared or the app is uninstalled, but this may vary depending on OS/backup policy.

#### (7) Local DB (Logs/Records) Storage (SQLite/sqflite)

Depending on the feature, the app may store the following **lottery record/log data** in a local DB.

- UI display values such as round information/date, selected number list, generation logs, and whether fingerprint use was enabled
- Purpose of use: record lookup, statistics calculation, and management of logs saved by the user
- Storage location: local DB inside the device
- Deletion: deleted together when app data is cleared or the app is uninstalled.

#### (8) Temporary Files/Cache

During normal operation, the following temporary data may be generated.

- Temporary data generated during JSON parsing
- Cache for UI rendering and library operation

Temporary files may be located in cache/temporary folder areas managed by the OS,  
may be automatically cleaned up according to OS policy, and are not uploaded to the developer's server.

---
