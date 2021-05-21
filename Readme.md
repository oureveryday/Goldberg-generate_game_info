# Goldberg Generate Game Info

A build and mod for goldberg Steam EMU generate_game_info.cpp
Normal:Steam API key needed
Mod xan105's api:Don't need steam API key(But can't generate items)

# Usage

generate_game_infos.exe app_id <-s steam_api_key> <-o output_path> <-p>
-s: Using steam API instead of xan105 API
-o: Output path(default is folder with app_id/steam_settings)
-p: Disable generate achievement photos

# Build

Run command on bash:
`g++ -o generate_game_infos generate_game_infos/generate_game_infos.cpp -lcurl`

Or on MinGW (Windows):
`g++ -o generate_game_infos.exe generate_game_infos/generate_game_infos.cpp -lcurl.dll`

Library requirment:
 * curl (https://github.com/curl/curl) or (https://curl.se/windows/)
 * json (https://github.com/nlohmann/json)
 * fifo_map (https://github.com/nlohmann/fifo_map)

# Thanks for the api,xan105！
