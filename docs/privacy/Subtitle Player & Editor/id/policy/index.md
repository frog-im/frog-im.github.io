## Third-party (modified)

- better_player 0.0.84 (Apache-2.0)
    - Original: https://pub.dev/packages/better_player
    - Local changes:
        - android/build.gradle: `namespace "com.jhomlala.better_player"` 추가 (AGP 8 대응)
        - lib/src/hls/hls_parser/hash_compat.dart: `hashValues` 대체 구현 추가 (`Object.hashAll` 기반)
        - lib/src/hls/hls_parser/drm_init_data.dart: `hash_compat.dart` import 및 로컬 `hashValues` 사용
        - lib/src/hls/hls_parser/hls_track_metadata_entry.dart: `hash_compat.dart` import 및 로컬 `hashValues` 사용
        - lib/src/hls/hls_parser/scheme_data.dart: `hash_compat.dart` import 및 로컬 `hashValues` 사용
        - lib/src/hls/hls_parser/variant_info.dart: `hash_compat.dart` import 및 로컬 `hashValues` 사용
