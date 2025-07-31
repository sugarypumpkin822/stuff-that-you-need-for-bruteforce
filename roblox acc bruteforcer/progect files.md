roblox_bruteforcer/
│
├── src/                                              # Core source code
│   ├── main.cpp                                       # Entry point
│   ├── bruteforcer.cpp                                # Bruteforce logic
│   ├── utils.cpp                                      # Utility functions
│   ├── logger.cpp                                     # Logging system
│   ├── config_loader.cpp                              # JSON config loading
│   ├── wordlist_loader.cpp                            # Loading wordlists
│   ├── network.cpp                                    # Simulates login requests
│   ├── statistics.cpp                                 # Keeps track of stats (e.g., attempts)
│   ├── captcha_solver.cpp                             # Captcha solving logic (if applicable)
│   ├── delay_handler.cpp                              # Handles rate-limiting and delays
│   ├── progress_bar.cpp                               # Progress bar management
│   ├── encryption.cpp                                 # For encrypted passwords (if required)
│   └── request_handler.cpp                            # Manages HTTP requests
│
├── include/                                            # Header files for each cpp file
│   ├── bruteforcer.h
│   ├── utils.h
│   ├── logger.h
│   ├── config_loader.h
│   ├── wordlist_loader.h
│   ├── statistics.h
│   ├── captcha_solver.h
│   ├── delay_handler.h
│   ├── progress_bar.h
│   ├── encryption.h
│   └── request_handler.h
│
├── wordlists/                                          # Wordlist files
│   ├── passwords.txt                                  # Default wordlist
│   ├── common.txt                                     # Common wordlist
│   ├── leaked_roblox_passwords.txt                    # Known leaked passwords
│   ├── custom_wordlist.txt                            # User-defined wordlist
│   └── hybrid_wordlist.txt                            # Combination of custom/common wordlist
│
├── tests/                                              # Unit & functional tests
│   ├── test_main.cpp                                   # Tests for main functionality
│   ├── test_utils.cpp                                  # Tests for utils
│   ├── test_config_loader.cpp                          # Tests for config loader
│   ├── test_wordlist_loader.cpp                        # Tests for wordlist loader
│   ├── test_logger.cpp                                 # Tests for logging system
│   ├── test_captcha_solver.cpp                         # Tests for captcha solving
│   ├── test_statistics.cpp                             # Tests for stats tracking
│   ├── test_delay_handler.cpp                          # Tests for rate-limiting
│   ├── test_progress_bar.cpp                           # Tests for progress bar
│   └── mocks/                                          # Mock classes for testing
│       └── mock_network.cpp                            # Fake network for testing
│
├── config/                                             # Configuration files
│   ├── config.json                                     # Main configuration settings
│   ├── debug_config.json                              # Debugging-specific config
│   ├── rate_limits.json                                # Rate limiting configurations
│   ├── captcha_config.json                            # Configuration for captcha solving
│   ├── encryption_config.json                         # Encryption options
│   └── proxy_config.json                              # Proxy settings for IP rotation
│
├── logs/                                               # Logging files
│   ├── bruteforcer.log                                 # Brute force attempts log
│   ├── error.log                                       # Error log
│   ├── debug.log                                       # Debug log
│   ├── request.log                                     # Logs HTTP requests
│   ├── response.log                                    # Logs responses from server
│   └── captcha.log                                     # Captcha solving attempts log
│
├── data/                                               # Data storage
│   ├── hits.csv                                        # Successful login hits
│   ├── statistics.json                                 # Brute force stats (e.g., attempts, success rate)
│   ├── failed_attempts.csv                             # Failed login attempts
│   └── user_data/                                      # User-related data storage
│       ├── session_data.json                           # Active session data
│       └── completed_attempts.json                     # Historical login attempts
│
├── scripts/                                            # Helper and automation scripts
│   ├── run.sh                                          # Bash script to run the project
│   ├── clean.sh                                        # Script to clean up logs/output
│   ├── build.sh                                        # Script to automate build process
│   ├── deploy.sh                                       # Deployment script (to cloud or other)
│   └── init.sh                                         # Initial setup (dependencies, environment variables)
│
├── docs/                                               # Documentation files
│   ├── README.md                                       # Project overview
│   ├── architecture.md                                 # Project architecture
│   ├── usage.md                                        # How to use the tool
│   ├── contributing.md                                # How to contribute to the project
│   ├── setup.md                                        # Setting up development environment
│   └── changelog.md                                    # Change log for versions
│
├── third_party/                                        # External dependencies
│   ├── json.hpp                                        # nlohmann/json single-header for JSON handling
│   └── libcurl/                                        # External library for HTTP requests
│
├── tools/                                              # Build and analysis tools
│   ├── formatter.cfg                                   # Code formatting configuration
│   ├── valgrind.supp                                   # Suppressions for valgrind
│   ├── static_analyzer.py                              # Python tool for static code analysis
│   └── code_coverage.sh                                # Shell script for code coverage reports
│
├── .gitignore                                          # Git ignore configuration
├── .clang-format                                       # Clang formatting config
├── CMakeLists.txt                                      # CMake build configuration file
├── LICENSE                                             # Project license (MIT, GPL, etc.)
└── version.txt                                         # Project version
