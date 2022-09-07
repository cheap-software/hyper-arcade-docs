# Hyper Arcade | Brainstorm 
## 1. Welcome page
**Functions:**
- redirect_to_login()
- redirect_to_signup()
- redirect_to_anonymus_menu()
- exit_game()

## 2. Login
**Form:**
- username
- password

**Functions:**
- validate_username(string username)
- encrypte_password(string password)
- validate_password(string enc_password)
- redirect_to_main()
- redirect_to_welcome_page()

## 3. Signup
**Form:**
- username
- password
- re_password

**Functions:**
- validate_username(string username)
- match_passwords(string password, string re_password)
- encrypte_password(string password)
- add_user(string username, string enc_password)
- redirect_to_main()
- redirect_to_welcome_page()

## 4. Main Menu
**Functions:**
- redirect_to_one_player_menu()
- redirect_to_multiplayer_menu()
- redirect_to_settings()
- redirect_to_about()
- [+] redirect_to_record()
- [+] logout()
    - redirect_to_welcome_page()
- [?] quit_menu()
    - redirect_to_welcome_page()

## 5. One Player Menu
**Functions:**
- select_game()
- redirect_to_one_player_game(int game_index)
- redirect_to_main()

## 6. Multiplayer Menu
**Functions:**
- redirect_to_join_room()
- redirect_to_create_room()
- redirect_to_main()

## 7. Join Room
**Form:**
- token

**Functions:**
- validate_token(string token)
- redirect_to_waiting_room()
- redirect_to_multiplayer_menu()

## 8. Waiting Room
**Functions:**
- select_game()
- redirect_to_multiplayer_game(int game_index)
- quit_room()
    - redirect_to_multiplayer_multiplayer_menu()

## 9. Create Room
**Functions:**
- generate_token()
- redirect_to_waiting_room()

## 10. Player Game (One/Multi)
**Functions:**
- play_game(int game_index)
    - dsepends on the game
- pause_game()
- intent_basic_settings()
- quit_game()
    - redirect_to_one_player_menu()

## 11. Basic Settings (Dialog)
**Functions:**
- select_lenguage()
- activate_noises()
- activate_music()
- change_controls()
- close_basic_settings()

## 12. Settings
**Functions:**
- select_lenguage()
- activate_noises()
- activate_music()
- selecte_theme()
- change_controls()
- [+] change_username(string new_username)
- [+] verify_username(string new_username)
- [+] change_password(string old_password, string new_password)
- [+] change_profile_picture(string image_base64)

## 13. About
**Functions:**
- display_about()
<br>

---
<br>

## Proposed Games
- Brick Ball
    - 1 player
- Wordle
    - 1 player
- Flappy Bird
    - 1 player
- Tetris
    - 1 player
- Tik Tak Toe
    - 2 players
- Hockey
    - 2 players
- Snake
    - 1 to 4 players
- Silly Raccon
    - 1 to 4 players

<br>

---
<br>

*Symbology*<br>
*[+] -> Requires session*<br>
*[?] -> Requires annonymous session*