# Comparing `tmp/voicegain-speech-1.84.0.tar.gz` & `tmp/voicegain-speech-1.84.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicegain-speech-1.84.0.tar", last modified: Tue Jun  6 18:31:47 2023, max compression
+gzip compressed data, was "voicegain-speech-1.84.1.tar", last modified: Wed Jun  7 19:40:03 2023, max compression
```

## Comparing `voicegain-speech-1.84.0.tar` & `voicegain-speech-1.84.1.tar`

### file list

```diff
@@ -1,478 +1,478 @@
-drwxr-xr-x   0     1001     1002        0 2023-06-06 18:31:47.243348 voicegain-speech-1.84.0/
--rw-r--r--   0     1001     1002    11357 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/LICENSE
--rw-r--r--   0     1001     1002     2923 2023-06-06 18:31:47.243348 voicegain-speech-1.84.0/PKG-INFO
--rw-r--r--   0     1001     1002     2491 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/README.md
--rw-r--r--   0     1001     1002       79 2023-06-06 18:31:47.243348 voicegain-speech-1.84.0/setup.cfg
--rw-r--r--   0     1001     1002      709 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/setup.py
-drwxr-xr-x   0     1001     1002        0 2023-06-06 18:31:47.143341 voicegain-speech-1.84.0/voicegain_speech/
--rw-r--r--   0     1001     1002    63204 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/__init__.py
-drwxr-xr-x   0     1001     1002        0 2023-06-06 18:31:47.151342 voicegain-speech-1.84.0/voicegain_speech/api/
--rw-r--r--   0     1001     1002      821 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/__init__.py
--rw-r--r--   0     1001     1002    33295 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/aivr_api.py
--rw-r--r--   0     1001     1002    52230 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/aivr_callback_api.py
--rw-r--r--   0     1001     1002    39238 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/asr_callback_api.py
--rw-r--r--   0     1001     1002    34610 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/audiocodes_api.py
--rw-r--r--   0     1001     1002   107540 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/data_api.py
--rw-r--r--   0     1001     1002   143653 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/greg_api.py
--rw-r--r--   0     1001     1002    63227 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/lm_api.py
--rw-r--r--   0     1001     1002    48176 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/recognize_api.py
--rw-r--r--   0     1001     1002   118989 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/sa_api.py
--rw-r--r--   0     1001     1002    37189 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/security_api.py
--rw-r--r--   0     1001     1002    57368 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/training_api.py
--rw-r--r--   0     1001     1002   103245 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/transcribe_api.py
--rw-r--r--   0     1001     1002    55743 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api/websocket_api.py
--rw-r--r--   0     1001     1002    51953 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/api_client.py
--rw-r--r--   0     1001     1002    38409 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/configuration.py
--rw-r--r--   0     1001     1002    30457 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/exceptions.py
-drwxr-xr-x   0     1001     1002        0 2023-06-06 18:31:47.243348 voicegain-speech-1.84.0/voicegain_speech/models/
--rw-r--r--   0     1001     1002    62020 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/__init__.py
--rw-r--r--   0     1001     1002    40146 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_control_messages.py
--rw-r--r--   0     1001     1002    31409 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_end.py
--rw-r--r--   0     1001     1002    31417 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_error.py
--rw-r--r--   0     1001     1002    31535 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_hypothesis.py
--rw-r--r--   0     1001     1002    30264 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_hypothesis_alternatives.py
--rw-r--r--   0     1001     1002    31505 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_recognition.py
--rw-r--r--   0     1001     1002    31668 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_recognition_alternatives.py
--rw-r--r--   0     1001     1002    32542 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_response_messages.py
--rw-r--r--   0     1001     1002    39629 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_start.py
--rw-r--r--   0     1001     1002    31681 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_start_stt_speech_contexts.py
--rw-r--r--   0     1001     1002    30534 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_started.py
--rw-r--r--   0     1001     1002    30603 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ac_stop.py
--rw-r--r--   0     1001     1002    31281 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/account_and_context_id.py
--rw-r--r--   0     1001     1002    34184 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/advanced_regex.py
--rw-r--r--   0     1001     1002    30211 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aircall.py
--rw-r--r--   0     1001     1002    30251 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aircall_all_of.py
--rw-r--r--   0     1001     1002    36150 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_callback_response.py
--rw-r--r--   0     1001     1002    31566 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_callback_response_final.py
--rw-r--r--   0     1001     1002    30228 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_conference_transfer.py
--rw-r--r--   0     1001     1002    30886 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_disconnect.py
--rw-r--r--   0     1001     1002    33824 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_event.py
--rw-r--r--   0     1001     1002    29629 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_event_type.py
--rw-r--r--   0     1001     1002    33087 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_existing_session.py
--rw-r--r--   0     1001     1002    32699 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_logic.py
--rw-r--r--   0     1001     1002    29492 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_logic_media.py
--rw-r--r--   0     1001     1002    31441 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_logic_transfer.py
--rw-r--r--   0     1001     1002    29578 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_logic_type.py
--rw-r--r--   0     1001     1002    41440 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_new_session.py
--rw-r--r--   0     1001     1002    30983 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_phone_transfer.py
--rw-r--r--   0     1001     1002    33973 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt.py
--rw-r--r--   0     1001     1002    30670 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt_completion.py
--rw-r--r--   0     1001     1002    35386 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt_playing.py
--rw-r--r--   0     1001     1002    30194 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt_properties_audio.py
--rw-r--r--   0     1001     1002    30204 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt_properties_html.py
--rw-r--r--   0     1001     1002    36851 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_question.py
--rw-r--r--   0     1001     1002    29589 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_recognition_result.py
--rw-r--r--   0     1001     1002    35656 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_recording.py
--rw-r--r--   0     1001     1002    41834 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_response_properties_audio.py
--rw-r--r--   0     1001     1002    31781 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_response_properties_html.py
--rw-r--r--   0     1001     1002    34451 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_session_user.py
--rw-r--r--   0     1001     1002    30557 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_session_user_base.py
--rw-r--r--   0     1001     1002    33323 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_session_user_fs.py
--rw-r--r--   0     1001     1002    32023 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivr_transfer.py
--rw-r--r--   0     1001     1002    32351 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/aivrs_question_specifics.py
--rw-r--r--   0     1001     1002    31631 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/answer_map_entry.py
--rw-r--r--   0     1001     1002    29583 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_event.py
--rw-r--r--   0     1001     1002    29674 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_status.py
--rw-r--r--   0     1001     1002    29594 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_status_additional.py
--rw-r--r--   0     1001     1002    29649 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_status_after_input_started.py
--rw-r--r--   0     1001     1002    29676 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_status_for_callback.py
--rw-r--r--   0     1001     1002    29585 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_recognition_result.py
--rw-r--r--   0     1001     1002    42888 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_common.py
--rw-r--r--   0     1001     1002    56904 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_recognition.py
--rw-r--r--   0     1001     1002    52268 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_recognition_defaults.py
--rw-r--r--   0     1001     1002    43581 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_recognition_grammars_etc.py
--rw-r--r--   0     1001     1002    38337 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_recognition_timeouts.py
--rw-r--r--   0     1001     1002    52356 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription.py
--rw-r--r--   0     1001     1002    59921 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_async.py
--rw-r--r--   0     1001     1002    31604 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_async_all_of.py
--rw-r--r--   0     1001     1002    50375 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_common.py
--rw-r--r--   0     1001     1002    36484 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_common_lm.py
--rw-r--r--   0     1001     1002    34663 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_default_timeouts.py
--rw-r--r--   0     1001     1002    55625 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_defaults.py
--rw-r--r--   0     1001     1002    51006 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_sa.py
--rw-r--r--   0     1001     1002    31790 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_speakers.py
--rw-r--r--   0     1001     1002    33207 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py
--rw-r--r--   0     1001     1002    34410 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/asr_transcribe_queue_status.py
--rw-r--r--   0     1001     1002    34139 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_audio_input_source.py
--rw-r--r--   0     1001     1002    29595 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_mode.py
--rw-r--r--   0     1001     1002    29639 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_mode_recognition.py
--rw-r--r--   0     1001     1002    29556 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_mode_speech_analytics.py
--rw-r--r--   0     1001     1002    29602 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_mode_transcription.py
--rw-r--r--   0     1001     1002    31776 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_post_response_base.py
--rw-r--r--   0     1001     1002    31171 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_post_response_base_audio.py
--rw-r--r--   0     1001     1002    32849 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_reco_post_response.py
--rw-r--r--   0     1001     1002    30526 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_reco_post_response_sessions.py
--rw-r--r--   0     1001     1002    30438 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_callback_response.py
--rw-r--r--   0     1001     1002    32070 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_request.py
--rw-r--r--   0     1001     1002    32200 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_response.py
--rw-r--r--   0     1001     1002    34959 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_result.py
--rw-r--r--   0     1001     1002    30225 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_result_all_of.py
--rw-r--r--   0     1001     1002    33787 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_full.py
--rw-r--r--   0     1001     1002    31696 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of.py
--rw-r--r--   0     1001     1002    30898 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_audio.py
--rw-r--r--   0     1001     1002    37213 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_audio_callback.py
--rw-r--r--   0     1001     1002    30312 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_audio_source.py
--rw-r--r--   0     1001     1002    30324 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py
--rw-r--r--   0     1001     1002    43657 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_result.py
--rw-r--r--   0     1001     1002    33328 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental.py
--rw-r--r--   0     1001     1002    31145 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental_detail.py
--rw-r--r--   0     1001     1002    31183 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental_detail_control_status.py
--rw-r--r--   0     1001     1002    39938 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental_detail_result.py
--rw-r--r--   0     1001     1002    34454 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py
--rw-r--r--   0     1001     1002    33330 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_session_established.py
--rw-r--r--   0     1001     1002    32712 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_session_short_info.py
--rw-r--r--   0     1001     1002    30339 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_session_url.py
--rw-r--r--   0     1001     1002    32907 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_transc_post_response.py
--rw-r--r--   0     1001     1002    30560 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_transc_post_response_sessions.py
--rw-r--r--   0     1001     1002    35405 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_transc_session_established.py
--rw-r--r--   0     1001     1002    30366 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_transcription_callback_response.py
--rw-r--r--   0     1001     1002    32007 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_transcription_request.py
--rw-r--r--   0     1001     1002    31380 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_transcription_response.py
--rw-r--r--   0     1001     1002    31808 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/async_transcription_response_shared.py
--rw-r--r--   0     1001     1002    29559 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_channel.py
--rw-r--r--   0     1001     1002    29537 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_channel_selector.py
--rw-r--r--   0     1001     1002    29630 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_channel_selector_offline_async.py
--rw-r--r--   0     1001     1002    29491 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_channels.py
--rw-r--r--   0     1001     1002    30186 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_for_data_object.py
--rw-r--r--   0     1001     1002    29606 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_format.py
--rw-r--r--   0     1001     1002    34037 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_async.py
--rw-r--r--   0     1001     1002    30252 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_async_source.py
--rw-r--r--   0     1001     1002    35159 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_async_with_callback.py
--rw-r--r--   0     1001     1002    33174 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_base.py
--rw-r--r--   0     1001     1002    30127 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_callback.py
--rw-r--r--   0     1001     1002    35290 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_callback_callback.py
--rw-r--r--   0     1001     1002    29361 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_data.py
--rw-r--r--   0     1001     1002    31543 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_data_all_of.py
--rw-r--r--   0     1001     1002    31443 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_data_all_of_source.py
--rw-r--r--   0     1001     1002    35000 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_sync.py
--rw-r--r--   0     1001     1002    31259 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_input_sync_source.py
--rw-r--r--   0     1001     1002    34471 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_resource_uri.py
--rw-r--r--   0     1001     1002    29591 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_zone_class.py
--rw-r--r--   0     1001     1002    31502 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/audio_zone_item.py
--rw-r--r--   0     1001     1002    30032 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/basic_success_response.py
--rw-r--r--   0     1001     1002    31534 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/builtin.py
--rw-r--r--   0     1001     1002    31594 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/builtin_all_of.py
--rw-r--r--   0     1001     1002    29873 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/call_attributes.py
--rw-r--r--   0     1001     1002    36588 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/call_review_answer_alone.py
--rw-r--r--   0     1001     1002    29522 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/call_review_answer_type.py
--rw-r--r--   0     1001     1002    33994 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/call_review_config_question_base.py
--rw-r--r--   0     1001     1002    43455 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/call_review_config_question_base_with_answer.py
--rw-r--r--   0     1001     1002    35752 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/call_review_config_question_base_with_id.py
--rw-r--r--   0     1001     1002    35241 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/callback_req.py
--rw-r--r--   0     1001     1002    31999 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/callback_req_reco.py
--rw-r--r--   0     1001     1002    30160 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/callback_resp.py
--rw-r--r--   0     1001     1002    33942 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/caption.py
--rw-r--r--   0     1001     1002    31002 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/compliance_settings.py
--rw-r--r--   0     1001     1002    29552 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/config_value_status.py
--rw-r--r--   0     1001     1002    29648 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/content_type.py
--rw-r--r--   0     1001     1002    33069 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/continuous_recognition.py
--rw-r--r--   0     1001     1002    50286 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/core_aivr_session.py
--rw-r--r--   0     1001     1002    39311 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/core_aivr_session_telco_data.py
--rw-r--r--   0     1001     1002    30991 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/cr_question_id_for_cr_config.py
--rw-r--r--   0     1001     1002    29516 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/creating_entity.py
--rw-r--r--   0     1001     1002    31201 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/criterion_config.py
--rw-r--r--   0     1001     1002    31102 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/criterion_satisfied.py
--rw-r--r--   0     1001     1002    30028 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/data_obj_ref.py
--rw-r--r--   0     1001     1002    44553 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/data_object.py
--rw-r--r--   0     1001     1002    30022 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/data_object_all_of.py
--rw-r--r--   0     1001     1002    38550 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/data_object_base.py
--rw-r--r--   0     1001     1002    34911 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/data_object_ids.py
--rw-r--r--   0     1001     1002    44332 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/data_object_no_sos_ref.py
--rw-r--r--   0     1001     1002    39523 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/data_object_with_audio.py
--rw-r--r--   0     1001     1002    29966 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/debug_info.py
--rw-r--r--   0     1001     1002    30572 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/debug_settings.py
--rw-r--r--   0     1001     1002    32571 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/demo.py
--rw-r--r--   0     1001     1002    32651 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/demo_all_of.py
--rw-r--r--   0     1001     1002    30958 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/diarization_data.py
--rw-r--r--   0     1001     1002    30827 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/diarization_zone.py
--rw-r--r--   0     1001     1002    36023 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/diarization_zone_item.py
--rw-r--r--   0     1001     1002    32689 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/disconnect.py
--rw-r--r--   0     1001     1002    32769 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/disconnect_all_of.py
--rw-r--r--   0     1001     1002    31021 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/error.py
--rw-r--r--   0     1001     1002    31081 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/error_all_of.py
--rw-r--r--   0     1001     1002    31069 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/error_info.py
--rw-r--r--   0     1001     1002    31630 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/estimated_queue_wait.py
--rw-r--r--   0     1001     1002    29571 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/experiment_platform.py
--rw-r--r--   0     1001     1002    32044 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/file_location.py
--rw-r--r--   0     1001     1002    35992 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/formatter.py
--rw-r--r--   0     1001     1002    30946 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/grammar.py
--rw-r--r--   0     1001     1002    30253 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg.py
--rw-r--r--   0     1001     1002    30293 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_all_of.py
--rw-r--r--   0     1001     1002    37404 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio.py
--rw-r--r--   0     1001     1002    31269 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_all_of.py
--rw-r--r--   0     1001     1002    32914 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_base.py
--rw-r--r--   0     1001     1002    33919 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_base_with_audio.py
--rw-r--r--   0     1001     1002    30259 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_id.py
--rw-r--r--   0     1001     1002    30911 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_input.py
--rw-r--r--   0     1001     1002    30241 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_input_audio_hash.py
--rw-r--r--   0     1001     1002    30159 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_input_audio_id.py
--rw-r--r--   0     1001     1002    30186 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_input_data.py
--rw-r--r--   0     1001     1002    34266 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set.py
--rw-r--r--   0     1001     1002    31589 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_base.py
--rw-r--r--   0     1001     1002    31662 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_base_inclusive.py
--rw-r--r--   0     1001     1002    32502 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_core.py
--rw-r--r--   0     1001     1002    30266 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_id.py
--rw-r--r--   0     1001     1002    32531 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_inclusive.py
--rw-r--r--   0     1001     1002    32611 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_inclusive_core.py
--rw-r--r--   0     1001     1002    32522 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_inner.py
--rw-r--r--   0     1001     1002    31360 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_response.py
--rw-r--r--   0     1001     1002    35728 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_thin.py
--rw-r--r--   0     1001     1002    38872 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment.py
--rw-r--r--   0     1001     1002    36229 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_base.py
--rw-r--r--   0     1001     1002    34965 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_base_inclusive.py
--rw-r--r--   0     1001     1002    31920 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_base_platform_data.py
--rw-r--r--   0     1001     1002    30304 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_id.py
--rw-r--r--   0     1001     1002    37732 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_inclusive.py
--rw-r--r--   0     1001     1002    35903 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_modifiable.py
--rw-r--r--   0     1001     1002    35527 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_platform_external_asr.py
--rw-r--r--   0     1001     1002    30570 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_platform_upload.py
--rw-r--r--   0     1001     1002    31282 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_platform_voicegain.py
--rw-r--r--   0     1001     1002    31388 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_response.py
--rw-r--r--   0     1001     1002    29672 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_status.py
--rw-r--r--   0     1001     1002    29601 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_status_modifiable.py
--rw-r--r--   0     1001     1002    34583 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar.py
--rw-r--r--   0     1001     1002    31855 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_base.py
--rw-r--r--   0     1001     1002    30859 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_base_light.py
--rw-r--r--   0     1001     1002    30321 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_id.py
--rw-r--r--   0     1001     1002    31787 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_inner.py
--rw-r--r--   0     1001     1002    33663 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_light.py
--rw-r--r--   0     1001     1002    30972 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_interpretation.py
--rw-r--r--   0     1001     1002    35202 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_question.py
--rw-r--r--   0     1001     1002    32455 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_question_base.py
--rw-r--r--   0     1001     1002    30352 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_question_id.py
--rw-r--r--   0     1001     1002    33478 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_question_inner.py
--rw-r--r--   0     1001     1002    31198 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py
--rw-r--r--   0     1001     1002    33674 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py
--rw-r--r--   0     1001     1002    31111 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py
--rw-r--r--   0     1001     1002    31041 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py
--rw-r--r--   0     1001     1002    30315 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_with_exp.py
--rw-r--r--   0     1001     1002    37164 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_recognition.py
--rw-r--r--   0     1001     1002    34456 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_recognition_base.py
--rw-r--r--   0     1001     1002    30333 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_recognition_id.py
--rw-r--r--   0     1001     1002    29620 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_review_status.py
--rw-r--r--   0     1001     1002    32583 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_source_of_truth.py
--rw-r--r--   0     1001     1002    33457 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_truth_update.py
--rw-r--r--   0     1001     1002    33217 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/greg_truth_updates.py
--rw-r--r--   0     1001     1002    32202 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/grxml.py
--rw-r--r--   0     1001     1002    32302 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/grxml_all_of.py
--rw-r--r--   0     1001     1002    30711 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/gui_input.py
--rw-r--r--   0     1001     1002    29329 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/hangup.py
--rw-r--r--   0     1001     1002    30001 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/html_checkbox.py
--rw-r--r--   0     1001     1002    31815 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/html_choice_item.py
--rw-r--r--   0     1001     1002    30033 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/html_radio_buttons.py
--rw-r--r--   0     1001     1002    30096 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/html_text_entry.py
--rw-r--r--   0     1001     1002    29489 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/if_exists.py
--rw-r--r--   0     1001     1002    33513 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/incident.py
--rw-r--r--   0     1001     1002    30020 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/inline_data.py
--rw-r--r--   0     1001     1002    31225 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/inline_object.py
--rw-r--r--   0     1001     1002    31237 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/inline_object1.py
--rw-r--r--   0     1001     1002    34640 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/input.py
--rw-r--r--   0     1001     1002    34780 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/input_all_of.py
--rw-r--r--   0     1001     1002    30940 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/integration.py
--rw-r--r--   0     1001     1002    36116 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/jjsgf.py
--rw-r--r--   0     1001     1002    36256 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/jjsgf_all_of.py
--rw-r--r--   0     1001     1002    31407 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/keyword_spot_example.py
--rw-r--r--   0     1001     1002    31392 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/keyword_spot_group.py
--rw-r--r--   0     1001     1002    33135 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/keyword_spot_item.py
--rw-r--r--   0     1001     1002    29613 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/lang_model_status.py
--rw-r--r--   0     1001     1002    30389 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/language.py
--rw-r--r--   0     1001     1002    39716 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/language_model_doc.py
--rw-r--r--   0     1001     1002    38173 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/language_model_doc_modifiable.py
--rw-r--r--   0     1001     1002    32931 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/language_model_src_data.py
--rw-r--r--   0     1001     1002    29490 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/lm_type.py
--rw-r--r--   0     1001     1002    30152 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/min_max_speakers.py
--rw-r--r--   0     1001     1002    32993 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/min_max_speakers_diarization.py
--rw-r--r--   0     1001     1002    29642 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/mood_type.py
--rw-r--r--   0     1001     1002    31485 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/mrc_pv1_asr_settings.py
--rw-r--r--   0     1001     1002    31458 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/mrc_pv2_asr_settings.py
--rw-r--r--   0     1001     1002    29489 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/mrcp_version.py
--rw-r--r--   0     1001     1002    33330 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/multipart_form_data_field.py
--rw-r--r--   0     1001     1002    31972 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/name_value_pair.py
--rw-r--r--   0     1001     1002    30984 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/named_entity_concept.py
--rw-r--r--   0     1001     1002    30105 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/named_entity_type.py
--rw-r--r--   0     1001     1002    49869 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/new_speech_analytics_session.py
--rw-r--r--   0     1001     1002    38283 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/new_speech_analytics_session_response.py
--rw-r--r--   0     1001     1002    30316 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/new_speech_analytics_session_response_poll.py
--rw-r--r--   0     1001     1002    30222 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/new_speech_analytics_session_response_websocket.py
--rw-r--r--   0     1001     1002    30870 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/non_session_error_response.py
--rw-r--r--   0     1001     1002    29409 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/non_session_error_response400.py
--rw-r--r--   0     1001     1002    29409 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/non_session_error_response401.py
--rw-r--r--   0     1001     1002    32303 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/output.py
--rw-r--r--   0     1001     1002    32383 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/output_all_of.py
--rw-r--r--   0     1001     1002    34585 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/overtalk.py
--rw-r--r--   0     1001     1002    32777 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/phone_audio_input.py
--rw-r--r--   0     1001     1002    30995 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/phone_audio_input_prompt.py
--rw-r--r--   0     1001     1002    33626 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_example.py
--rw-r--r--   0     1001     1002    33492 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_group.py
--rw-r--r--   0     1001     1002    41135 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_item.py
--rw-r--r--   0     1001     1002    32456 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_item_location.py
--rw-r--r--   0     1001     1002    32236 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_item_location_dialogue.py
--rw-r--r--   0     1001     1002    31096 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_item_slots.py
--rw-r--r--   0     1001     1002    33032 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/pii_redaction_conf.py
--rw-r--r--   0     1001     1002    33834 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/poll_req.py
--rw-r--r--   0     1001     1002    33610 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/poll_resp.py
--rw-r--r--   0     1001     1002    33580 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/portal_output_init.py
--rw-r--r--   0     1001     1002    30369 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/pre_fetch.py
--rw-r--r--   0     1001     1002    41038 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/progress.py
--rw-r--r--   0     1001     1002    31854 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/progress_callback.py
--rw-r--r--   0     1001     1002    29776 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/progress_phase.py
--rw-r--r--   0     1001     1002    32898 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/quartiles_energy.py
--rw-r--r--   0     1001     1002    32874 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/quartiles_pitch.py
--rw-r--r--   0     1001     1002    34683 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/reco_alt.py
--rw-r--r--   0     1001     1002    31884 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/recog_nlsml.py
--rw-r--r--   0     1001     1002    31054 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/recog_nlsml_no_exp.py
--rw-r--r--   0     1001     1002    34148 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/recog_obj.py
--rw-r--r--   0     1001     1002    33386 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/recog_obj_no_exp.py
--rw-r--r--   0     1001     1002    34047 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/recognition_result.py
--rw-r--r--   0     1001     1002    34316 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/requested_content.py
--rw-r--r--   0     1001     1002    33327 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/resource_uri.py
--rw-r--r--   0     1001     1002    29579 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/results_websocket_mode.py
--rw-r--r--   0     1001     1002    35226 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/s3.py
--rw-r--r--   0     1001     1002    35386 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/s3_all_of.py
--rw-r--r--   0     1001     1002    35343 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/s3_audio_input.py
--rw-r--r--   0     1001     1002    31594 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/s3_metadata_mapping.py
--rw-r--r--   0     1001     1002    31372 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/s3_tag_mapping.py
--rw-r--r--   0     1001     1002    29506 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sa_conf_type.py
--rw-r--r--   0     1001     1002    29625 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sample_rate.py
--rw-r--r--   0     1001     1002    35577 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sentence_hypothesis_or_recognition.py
--rw-r--r--   0     1001     1002    31912 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sentence_hypothesis_or_recognition_alternatives.py
--rw-r--r--   0     1001     1002    34034 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sentence_recognition.py
--rw-r--r--   0     1001     1002    30202 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/session_content.py
--rw-r--r--   0     1001     1002    31714 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/session_error_response.py
--rw-r--r--   0     1001     1002    37730 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/session_init_recognition.py
--rw-r--r--   0     1001     1002    39972 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/session_init_transcription.py
--rw-r--r--   0     1001     1002    33134 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/session_init_transcription_diarization.py
--rw-r--r--   0     1001     1002    30936 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/session_success_response.py
--rw-r--r--   0     1001     1002    35545 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/settings_async_transcription.py
--rw-r--r--   0     1001     1002    32466 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/settings_recognition.py
--rw-r--r--   0     1001     1002    32439 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/settings_sync_transcription.py
--rw-r--r--   0     1001     1002    34451 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/silence.py
--rw-r--r--   0     1001     1002    31097 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/slot_entity.py
--rw-r--r--   0     1001     1002    31044 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/slot_keyword.py
--rw-r--r--   0     1001     1002    31131 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sos_ref.py
--rw-r--r--   0     1001     1002    33790 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speaker_result.py
--rw-r--r--   0     1001     1002    44598 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_base_result.py
--rw-r--r--   0     1001     1002    32273 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_channel.py
--rw-r--r--   0     1001     1002    45971 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_channel_result.py
--rw-r--r--   0     1001     1002    34257 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_channel_with_transcribe.py
--rw-r--r--   0     1001     1002    71029 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config.py
--rw-r--r--   0     1001     1002    34715 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_identifying.py
--rw-r--r--   0     1001     1002    68304 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_modifiable.py
--rw-r--r--   0     1001     1002    67024 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_modifiable_base.py
--rw-r--r--   0     1001     1002    31582 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py
--rw-r--r--   0     1001     1002    31125 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_name_optional.py
--rw-r--r--   0     1001     1002    31279 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_name_required.py
--rw-r--r--   0     1001     1002    50325 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_core_result.py
--rw-r--r--   0     1001     1002    35252 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_core_result_all_of.py
--rw-r--r--   0     1001     1002    31191 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_criteria_data.py
--rw-r--r--   0     1001     1002    31656 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_emotion.py
--rw-r--r--   0     1001     1002    30859 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_emotion_data.py
--rw-r--r--   0     1001     1002    36980 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_emotion_item.py
--rw-r--r--   0     1001     1002    30905 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword.py
--rw-r--r--   0     1001     1002    31195 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword_data.py
--rw-r--r--   0     1001     1002    36229 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword_item.py
--rw-r--r--   0     1001     1002    36481 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py
--rw-r--r--   0     1001     1002    32743 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py
--rw-r--r--   0     1001     1002    31875 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_named_entity.py
--rw-r--r--   0     1001     1002    37279 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_named_entity_item.py
--rw-r--r--   0     1001     1002    37567 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py
--rw-r--r--   0     1001     1002    33817 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py
--rw-r--r--   0     1001     1002    32961 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase.py
--rw-r--r--   0     1001     1002    31178 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_data.py
--rw-r--r--   0     1001     1002    33076 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_for_ws.py
--rw-r--r--   0     1001     1002    31165 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py
--rw-r--r--   0     1001     1002    31004 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_group.py
--rw-r--r--   0     1001     1002    31277 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_group_data.py
--rw-r--r--   0     1001     1002    31037 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py
--rw-r--r--   0     1001     1002    36392 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_group_item.py
--rw-r--r--   0     1001     1002    38301 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_item.py
--rw-r--r--   0     1001     1002    39701 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py
--rw-r--r--   0     1001     1002    31075 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_slots.py
--rw-r--r--   0     1001     1002    61305 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_result.py
--rw-r--r--   0     1001     1002    46632 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_result_detail.py
--rw-r--r--   0     1001     1002    31090 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_session_modifiable.py
--rw-r--r--   0     1001     1002    38025 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_session_poll_response.py
--rw-r--r--   0     1001     1002    36320 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_websocket_payload.py
--rw-r--r--   0     1001     1002    31727 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/start_end_time_for_sub_criterion.py
--rw-r--r--   0     1001     1002    30413 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/stomp_ping.py
--rw-r--r--   0     1001     1002    33033 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/stomp_word_correction.py
--rw-r--r--   0     1001     1002    37052 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/stomp_ws_word.py
--rw-r--r--   0     1001     1002    31190 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/stomp_ws_word_all_of.py
--rw-r--r--   0     1001     1002    35347 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/stomp_ws_word_base.py
--rw-r--r--   0     1001     1002    35619 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/stream_resp.py
--rw-r--r--   0     1001     1002    33180 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/stream_setup.py
--rw-r--r--   0     1001     1002    29633 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/streaming_protocol.py
--rw-r--r--   0     1001     1002    38812 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sub_criterion_config.py
--rw-r--r--   0     1001     1002    41198 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sub_criterion_satisfied.py
--rw-r--r--   0     1001     1002    32173 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sync_audio_input_source.py
--rw-r--r--   0     1001     1002    31121 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sync_recognition_request.py
--rw-r--r--   0     1001     1002    32686 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sync_recognition_response.py
--rw-r--r--   0     1001     1002    30289 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sync_session_established.py
--rw-r--r--   0     1001     1002    31005 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sync_transcription_request.py
--rw-r--r--   0     1001     1002    32744 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sync_transcription_response.py
--rw-r--r--   0     1001     1002    33183 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/sync_transcription_result.py
--rw-r--r--   0     1001     1002    38899 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/talk_time.py
--rw-r--r--   0     1001     1002    31430 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/topic_score.py
--rw-r--r--   0     1001     1002    29529 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_bucket_type.py
--rw-r--r--   0     1001     1002    39171 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_doc.py
--rw-r--r--   0     1001     1002    31089 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_doc_defaults.py
--rw-r--r--   0     1001     1002    36549 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_doc_statistics.py
--rw-r--r--   0     1001     1002    34623 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_key.py
--rw-r--r--   0     1001     1002    33873 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_modifiable.py
--rw-r--r--   0     1001     1002    29621 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_status.py
--rw-r--r--   0     1001     1002    29661 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_status_modifiable.py
--rw-r--r--   0     1001     1002    29549 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/training_set_store_type.py
--rw-r--r--   0     1001     1002    31791 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transcribe_alt.py
--rw-r--r--   0     1001     1002    31073 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transcribe_session_id.py
--rw-r--r--   0     1001     1002    34091 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transcribe_session_modify_request.py
--rw-r--r--   0     1001     1002    31768 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transcribe_session_modify_request_mute.py
--rw-r--r--   0     1001     1002    30596 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transcribe_session_modify_request_pause.py
--rw-r--r--   0     1001     1002    34625 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transcript_position_range.py
--rw-r--r--   0     1001     1002    34805 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transcript_position_range_for_phrase.py
--rw-r--r--   0     1001     1002    36041 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py
--rw-r--r--   0     1001     1002    36362 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transfer.py
--rw-r--r--   0     1001     1002    36502 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/transfer_all_of.py
--rw-r--r--   0     1001     1002    29545 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/vad_mode.py
--rw-r--r--   0     1001     1002    32350 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/version.py
--rw-r--r--   0     1001     1002    38002 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/websocket.py
--rw-r--r--   0     1001     1002    41056 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/websocket_init.py
--rw-r--r--   0     1001     1002    30563 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/websocket_init_reco.py
--rw-r--r--   0     1001     1002    36158 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/websocket_modifiable.py
--rw-r--r--   0     1001     1002    32626 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/websocket_msg.py
--rw-r--r--   0     1001     1002    29492 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/websocket_protocol.py
--rw-r--r--   0     1001     1002    30967 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/websocket_resp.py
--rw-r--r--   0     1001     1002    30324 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/word_alternatives.py
--rw-r--r--   0     1001     1002    31504 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/word_cloud_item.py
--rw-r--r--   0     1001     1002    31345 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/word_correction.py
--rw-r--r--   0     1001     1002    36355 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/word_item_timed.py
--rw-r--r--   0     1001     1002    31430 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/word_item_timing.py
--rw-r--r--   0     1001     1002    30685 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/word_tree_ids.py
--rw-r--r--   0     1001     1002    36732 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/word_tree_item.py
--rw-r--r--   0     1001     1002    33287 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/words_item.py
--rw-r--r--   0     1001     1002    36590 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/words_section.py
--rw-r--r--   0     1001     1002    33136 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/words_section_meta.py
--rw-r--r--   0     1001     1002    32138 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/words_section_meta_mc.py
--rw-r--r--   0     1001     1002    34117 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/words_section_single_column.py
--rw-r--r--   0     1001     1002    30198 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/words_section_words.py
--rw-r--r--   0     1001     1002    44223 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/words_websocket_item.py
--rw-r--r--   0     1001     1002    33874 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_emotion_item.py
--rw-r--r--   0     1001     1002    33123 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_keyword_item.py
--rw-r--r--   0     1001     1002    34113 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_named_entity_item.py
--rw-r--r--   0     1001     1002    32347 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_phrase_group_item.py
--rw-r--r--   0     1001     1002    35126 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_phrase_item.py
--rw-r--r--   0     1001     1002    35478 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_phrase_item_inside_group.py
--rw-r--r--   0     1001     1002    31699 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_position_range.py
--rw-r--r--   0     1001     1002    30883 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_position_range_nested.py
--rw-r--r--   0     1001     1002    30871 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_position_range_no_spk.py
--rw-r--r--   0     1001     1002    37496 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py
--rw-r--r--   0     1001     1002    31348 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py
--rw-r--r--   0     1001     1002    32681 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_speaker.py
--rw-r--r--   0     1001     1002    34541 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_word.py
--rw-r--r--   0     1001     1002    32107 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/models/ws_word_edit.py
--rw-r--r--   0     1001     1002    39168 2023-06-06 18:31:44.000000 voicegain-speech-1.84.0/voicegain_speech/rest.py
-drwxr-xr-x   0     1001     1002        0 2023-06-06 18:31:47.147342 voicegain-speech-1.84.0/voicegain_speech.egg-info/
--rw-r--r--   0     1001     1002     2923 2023-06-06 18:31:47.000000 voicegain-speech-1.84.0/voicegain_speech.egg-info/PKG-INFO
--rw-r--r--   0     1001     1002    22939 2023-06-06 18:31:47.000000 voicegain-speech-1.84.0/voicegain_speech.egg-info/SOURCES.txt
--rw-r--r--   0     1001     1002        1 2023-06-06 18:31:47.000000 voicegain-speech-1.84.0/voicegain_speech.egg-info/dependency_links.txt
--rw-r--r--   0     1001     1002       48 2023-06-06 18:31:47.000000 voicegain-speech-1.84.0/voicegain_speech.egg-info/requires.txt
--rw-r--r--   0     1001     1002       17 2023-06-06 18:31:47.000000 voicegain-speech-1.84.0/voicegain_speech.egg-info/top_level.txt
+drwxr-xr-x   0     1001     1002        0 2023-06-07 19:40:03.673648 voicegain-speech-1.84.1/
+-rw-r--r--   0     1001     1002    11357 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/LICENSE
+-rw-r--r--   0     1001     1002     2923 2023-06-07 19:40:03.677649 voicegain-speech-1.84.1/PKG-INFO
+-rw-r--r--   0     1001     1002     2491 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/README.md
+-rw-r--r--   0     1001     1002       79 2023-06-07 19:40:03.677649 voicegain-speech-1.84.1/setup.cfg
+-rw-r--r--   0     1001     1002      709 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/setup.py
+drwxr-xr-x   0     1001     1002        0 2023-06-07 19:40:03.597644 voicegain-speech-1.84.1/voicegain_speech/
+-rw-r--r--   0     1001     1002    63204 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/__init__.py
+drwxr-xr-x   0     1001     1002        0 2023-06-07 19:40:03.601644 voicegain-speech-1.84.1/voicegain_speech/api/
+-rw-r--r--   0     1001     1002      821 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/__init__.py
+-rw-r--r--   0     1001     1002    33295 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/aivr_api.py
+-rw-r--r--   0     1001     1002    52230 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/aivr_callback_api.py
+-rw-r--r--   0     1001     1002    39238 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/asr_callback_api.py
+-rw-r--r--   0     1001     1002    34610 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/audiocodes_api.py
+-rw-r--r--   0     1001     1002   107540 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/data_api.py
+-rw-r--r--   0     1001     1002   143653 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/greg_api.py
+-rw-r--r--   0     1001     1002    63227 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/lm_api.py
+-rw-r--r--   0     1001     1002    48176 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/recognize_api.py
+-rw-r--r--   0     1001     1002   118989 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/sa_api.py
+-rw-r--r--   0     1001     1002    37189 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/security_api.py
+-rw-r--r--   0     1001     1002    57368 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/training_api.py
+-rw-r--r--   0     1001     1002   103245 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/transcribe_api.py
+-rw-r--r--   0     1001     1002    55743 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api/websocket_api.py
+-rw-r--r--   0     1001     1002    51953 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/api_client.py
+-rw-r--r--   0     1001     1002    38409 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/configuration.py
+-rw-r--r--   0     1001     1002    30457 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/exceptions.py
+drwxr-xr-x   0     1001     1002        0 2023-06-07 19:40:03.673648 voicegain-speech-1.84.1/voicegain_speech/models/
+-rw-r--r--   0     1001     1002    62020 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/__init__.py
+-rw-r--r--   0     1001     1002    40146 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_control_messages.py
+-rw-r--r--   0     1001     1002    31409 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_end.py
+-rw-r--r--   0     1001     1002    31417 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_error.py
+-rw-r--r--   0     1001     1002    31535 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_hypothesis.py
+-rw-r--r--   0     1001     1002    30264 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_hypothesis_alternatives.py
+-rw-r--r--   0     1001     1002    31505 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_recognition.py
+-rw-r--r--   0     1001     1002    31668 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_recognition_alternatives.py
+-rw-r--r--   0     1001     1002    32542 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_response_messages.py
+-rw-r--r--   0     1001     1002    39629 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_start.py
+-rw-r--r--   0     1001     1002    31681 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_start_stt_speech_contexts.py
+-rw-r--r--   0     1001     1002    30534 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_started.py
+-rw-r--r--   0     1001     1002    30603 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ac_stop.py
+-rw-r--r--   0     1001     1002    31281 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/account_and_context_id.py
+-rw-r--r--   0     1001     1002    34184 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/advanced_regex.py
+-rw-r--r--   0     1001     1002    30211 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aircall.py
+-rw-r--r--   0     1001     1002    30251 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aircall_all_of.py
+-rw-r--r--   0     1001     1002    36150 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_callback_response.py
+-rw-r--r--   0     1001     1002    31566 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_callback_response_final.py
+-rw-r--r--   0     1001     1002    30228 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_conference_transfer.py
+-rw-r--r--   0     1001     1002    30886 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_disconnect.py
+-rw-r--r--   0     1001     1002    33824 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_event.py
+-rw-r--r--   0     1001     1002    29629 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_event_type.py
+-rw-r--r--   0     1001     1002    33087 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_existing_session.py
+-rw-r--r--   0     1001     1002    32699 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_logic.py
+-rw-r--r--   0     1001     1002    29492 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_logic_media.py
+-rw-r--r--   0     1001     1002    31441 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_logic_transfer.py
+-rw-r--r--   0     1001     1002    29578 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_logic_type.py
+-rw-r--r--   0     1001     1002    41440 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_new_session.py
+-rw-r--r--   0     1001     1002    30983 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_phone_transfer.py
+-rw-r--r--   0     1001     1002    33973 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt.py
+-rw-r--r--   0     1001     1002    30670 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt_completion.py
+-rw-r--r--   0     1001     1002    35386 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt_playing.py
+-rw-r--r--   0     1001     1002    30194 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt_properties_audio.py
+-rw-r--r--   0     1001     1002    30204 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt_properties_html.py
+-rw-r--r--   0     1001     1002    36851 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_question.py
+-rw-r--r--   0     1001     1002    29589 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_recognition_result.py
+-rw-r--r--   0     1001     1002    35656 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_recording.py
+-rw-r--r--   0     1001     1002    41834 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_response_properties_audio.py
+-rw-r--r--   0     1001     1002    31781 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_response_properties_html.py
+-rw-r--r--   0     1001     1002    34451 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_session_user.py
+-rw-r--r--   0     1001     1002    30557 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_session_user_base.py
+-rw-r--r--   0     1001     1002    33323 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_session_user_fs.py
+-rw-r--r--   0     1001     1002    32023 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivr_transfer.py
+-rw-r--r--   0     1001     1002    32351 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/aivrs_question_specifics.py
+-rw-r--r--   0     1001     1002    31631 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/answer_map_entry.py
+-rw-r--r--   0     1001     1002    29583 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_event.py
+-rw-r--r--   0     1001     1002    29674 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_status.py
+-rw-r--r--   0     1001     1002    29594 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_status_additional.py
+-rw-r--r--   0     1001     1002    29649 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_status_after_input_started.py
+-rw-r--r--   0     1001     1002    29676 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_status_for_callback.py
+-rw-r--r--   0     1001     1002    29585 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_recognition_result.py
+-rw-r--r--   0     1001     1002    42888 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_common.py
+-rw-r--r--   0     1001     1002    56904 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_recognition.py
+-rw-r--r--   0     1001     1002    52268 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_recognition_defaults.py
+-rw-r--r--   0     1001     1002    43581 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_recognition_grammars_etc.py
+-rw-r--r--   0     1001     1002    38337 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_recognition_timeouts.py
+-rw-r--r--   0     1001     1002    52356 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription.py
+-rw-r--r--   0     1001     1002    59921 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_async.py
+-rw-r--r--   0     1001     1002    31604 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_async_all_of.py
+-rw-r--r--   0     1001     1002    50375 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_common.py
+-rw-r--r--   0     1001     1002    36484 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_common_lm.py
+-rw-r--r--   0     1001     1002    34663 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_default_timeouts.py
+-rw-r--r--   0     1001     1002    55625 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_defaults.py
+-rw-r--r--   0     1001     1002    51006 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_sa.py
+-rw-r--r--   0     1001     1002    31790 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_speakers.py
+-rw-r--r--   0     1001     1002    33207 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py
+-rw-r--r--   0     1001     1002    34410 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/asr_transcribe_queue_status.py
+-rw-r--r--   0     1001     1002    34139 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_audio_input_source.py
+-rw-r--r--   0     1001     1002    29595 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_mode.py
+-rw-r--r--   0     1001     1002    29639 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_mode_recognition.py
+-rw-r--r--   0     1001     1002    29556 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_mode_speech_analytics.py
+-rw-r--r--   0     1001     1002    29602 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_mode_transcription.py
+-rw-r--r--   0     1001     1002    31776 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_post_response_base.py
+-rw-r--r--   0     1001     1002    31171 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_post_response_base_audio.py
+-rw-r--r--   0     1001     1002    32849 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_reco_post_response.py
+-rw-r--r--   0     1001     1002    30526 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_reco_post_response_sessions.py
+-rw-r--r--   0     1001     1002    30438 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_callback_response.py
+-rw-r--r--   0     1001     1002    32070 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_request.py
+-rw-r--r--   0     1001     1002    32200 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_response.py
+-rw-r--r--   0     1001     1002    34959 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_result.py
+-rw-r--r--   0     1001     1002    30225 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_result_all_of.py
+-rw-r--r--   0     1001     1002    33787 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_full.py
+-rw-r--r--   0     1001     1002    31696 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of.py
+-rw-r--r--   0     1001     1002    30898 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_audio.py
+-rw-r--r--   0     1001     1002    37213 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_audio_callback.py
+-rw-r--r--   0     1001     1002    30312 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_audio_source.py
+-rw-r--r--   0     1001     1002    30324 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py
+-rw-r--r--   0     1001     1002    43657 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_result.py
+-rw-r--r--   0     1001     1002    33328 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental.py
+-rw-r--r--   0     1001     1002    31145 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental_detail.py
+-rw-r--r--   0     1001     1002    31183 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental_detail_control_status.py
+-rw-r--r--   0     1001     1002    39938 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental_detail_result.py
+-rw-r--r--   0     1001     1002    34454 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py
+-rw-r--r--   0     1001     1002    33330 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_session_established.py
+-rw-r--r--   0     1001     1002    32712 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_session_short_info.py
+-rw-r--r--   0     1001     1002    30339 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_session_url.py
+-rw-r--r--   0     1001     1002    32907 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_transc_post_response.py
+-rw-r--r--   0     1001     1002    30560 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_transc_post_response_sessions.py
+-rw-r--r--   0     1001     1002    35405 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_transc_session_established.py
+-rw-r--r--   0     1001     1002    30366 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_transcription_callback_response.py
+-rw-r--r--   0     1001     1002    32007 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_transcription_request.py
+-rw-r--r--   0     1001     1002    31380 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_transcription_response.py
+-rw-r--r--   0     1001     1002    31808 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/async_transcription_response_shared.py
+-rw-r--r--   0     1001     1002    29559 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_channel.py
+-rw-r--r--   0     1001     1002    29537 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_channel_selector.py
+-rw-r--r--   0     1001     1002    29630 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_channel_selector_offline_async.py
+-rw-r--r--   0     1001     1002    29491 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_channels.py
+-rw-r--r--   0     1001     1002    30186 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_for_data_object.py
+-rw-r--r--   0     1001     1002    29606 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_format.py
+-rw-r--r--   0     1001     1002    34037 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_async.py
+-rw-r--r--   0     1001     1002    30252 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_async_source.py
+-rw-r--r--   0     1001     1002    35159 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_async_with_callback.py
+-rw-r--r--   0     1001     1002    33174 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_base.py
+-rw-r--r--   0     1001     1002    30127 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_callback.py
+-rw-r--r--   0     1001     1002    35290 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_callback_callback.py
+-rw-r--r--   0     1001     1002    29361 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_data.py
+-rw-r--r--   0     1001     1002    31543 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_data_all_of.py
+-rw-r--r--   0     1001     1002    31443 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_data_all_of_source.py
+-rw-r--r--   0     1001     1002    35000 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_sync.py
+-rw-r--r--   0     1001     1002    31259 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_input_sync_source.py
+-rw-r--r--   0     1001     1002    34471 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_resource_uri.py
+-rw-r--r--   0     1001     1002    29591 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_zone_class.py
+-rw-r--r--   0     1001     1002    31502 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/audio_zone_item.py
+-rw-r--r--   0     1001     1002    30032 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/basic_success_response.py
+-rw-r--r--   0     1001     1002    31534 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/builtin.py
+-rw-r--r--   0     1001     1002    31594 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/builtin_all_of.py
+-rw-r--r--   0     1001     1002    29873 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/call_attributes.py
+-rw-r--r--   0     1001     1002    36588 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/call_review_answer_alone.py
+-rw-r--r--   0     1001     1002    29522 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/call_review_answer_type.py
+-rw-r--r--   0     1001     1002    33994 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/call_review_config_question_base.py
+-rw-r--r--   0     1001     1002    43455 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/call_review_config_question_base_with_answer.py
+-rw-r--r--   0     1001     1002    35752 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/call_review_config_question_base_with_id.py
+-rw-r--r--   0     1001     1002    35241 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/callback_req.py
+-rw-r--r--   0     1001     1002    31999 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/callback_req_reco.py
+-rw-r--r--   0     1001     1002    30160 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/callback_resp.py
+-rw-r--r--   0     1001     1002    33942 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/caption.py
+-rw-r--r--   0     1001     1002    31002 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/compliance_settings.py
+-rw-r--r--   0     1001     1002    29552 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/config_value_status.py
+-rw-r--r--   0     1001     1002    29648 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/content_type.py
+-rw-r--r--   0     1001     1002    33069 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/continuous_recognition.py
+-rw-r--r--   0     1001     1002    50286 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/core_aivr_session.py
+-rw-r--r--   0     1001     1002    39311 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/core_aivr_session_telco_data.py
+-rw-r--r--   0     1001     1002    30991 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/cr_question_id_for_cr_config.py
+-rw-r--r--   0     1001     1002    29516 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/creating_entity.py
+-rw-r--r--   0     1001     1002    31201 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/criterion_config.py
+-rw-r--r--   0     1001     1002    31102 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/criterion_satisfied.py
+-rw-r--r--   0     1001     1002    30028 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/data_obj_ref.py
+-rw-r--r--   0     1001     1002    44553 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/data_object.py
+-rw-r--r--   0     1001     1002    30022 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/data_object_all_of.py
+-rw-r--r--   0     1001     1002    38550 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/data_object_base.py
+-rw-r--r--   0     1001     1002    34911 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/data_object_ids.py
+-rw-r--r--   0     1001     1002    44332 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/data_object_no_sos_ref.py
+-rw-r--r--   0     1001     1002    39523 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/data_object_with_audio.py
+-rw-r--r--   0     1001     1002    29966 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/debug_info.py
+-rw-r--r--   0     1001     1002    30572 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/debug_settings.py
+-rw-r--r--   0     1001     1002    32571 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/demo.py
+-rw-r--r--   0     1001     1002    32651 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/demo_all_of.py
+-rw-r--r--   0     1001     1002    30958 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/diarization_data.py
+-rw-r--r--   0     1001     1002    30827 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/diarization_zone.py
+-rw-r--r--   0     1001     1002    36023 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/diarization_zone_item.py
+-rw-r--r--   0     1001     1002    32689 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/disconnect.py
+-rw-r--r--   0     1001     1002    32769 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/disconnect_all_of.py
+-rw-r--r--   0     1001     1002    31021 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/error.py
+-rw-r--r--   0     1001     1002    31081 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/error_all_of.py
+-rw-r--r--   0     1001     1002    31069 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/error_info.py
+-rw-r--r--   0     1001     1002    31630 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/estimated_queue_wait.py
+-rw-r--r--   0     1001     1002    29571 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/experiment_platform.py
+-rw-r--r--   0     1001     1002    32044 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/file_location.py
+-rw-r--r--   0     1001     1002    35992 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/formatter.py
+-rw-r--r--   0     1001     1002    30946 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/grammar.py
+-rw-r--r--   0     1001     1002    30253 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg.py
+-rw-r--r--   0     1001     1002    30293 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_all_of.py
+-rw-r--r--   0     1001     1002    37404 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio.py
+-rw-r--r--   0     1001     1002    31269 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_all_of.py
+-rw-r--r--   0     1001     1002    32914 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_base.py
+-rw-r--r--   0     1001     1002    33919 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_base_with_audio.py
+-rw-r--r--   0     1001     1002    30259 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_id.py
+-rw-r--r--   0     1001     1002    30911 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_input.py
+-rw-r--r--   0     1001     1002    30241 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_input_audio_hash.py
+-rw-r--r--   0     1001     1002    30159 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_input_audio_id.py
+-rw-r--r--   0     1001     1002    30186 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_input_data.py
+-rw-r--r--   0     1001     1002    34266 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set.py
+-rw-r--r--   0     1001     1002    31589 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_base.py
+-rw-r--r--   0     1001     1002    31662 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_base_inclusive.py
+-rw-r--r--   0     1001     1002    32502 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_core.py
+-rw-r--r--   0     1001     1002    30266 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_id.py
+-rw-r--r--   0     1001     1002    32531 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_inclusive.py
+-rw-r--r--   0     1001     1002    32611 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_inclusive_core.py
+-rw-r--r--   0     1001     1002    32522 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_inner.py
+-rw-r--r--   0     1001     1002    31360 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_response.py
+-rw-r--r--   0     1001     1002    35728 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_thin.py
+-rw-r--r--   0     1001     1002    38872 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment.py
+-rw-r--r--   0     1001     1002    36229 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_base.py
+-rw-r--r--   0     1001     1002    34965 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_base_inclusive.py
+-rw-r--r--   0     1001     1002    31920 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_base_platform_data.py
+-rw-r--r--   0     1001     1002    30304 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_id.py
+-rw-r--r--   0     1001     1002    37732 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_inclusive.py
+-rw-r--r--   0     1001     1002    35903 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_modifiable.py
+-rw-r--r--   0     1001     1002    35527 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_platform_external_asr.py
+-rw-r--r--   0     1001     1002    30570 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_platform_upload.py
+-rw-r--r--   0     1001     1002    31282 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_platform_voicegain.py
+-rw-r--r--   0     1001     1002    31388 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_response.py
+-rw-r--r--   0     1001     1002    29672 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_status.py
+-rw-r--r--   0     1001     1002    29601 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_status_modifiable.py
+-rw-r--r--   0     1001     1002    34583 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar.py
+-rw-r--r--   0     1001     1002    31855 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_base.py
+-rw-r--r--   0     1001     1002    30859 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_base_light.py
+-rw-r--r--   0     1001     1002    30321 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_id.py
+-rw-r--r--   0     1001     1002    31787 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_inner.py
+-rw-r--r--   0     1001     1002    33663 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_light.py
+-rw-r--r--   0     1001     1002    30972 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_interpretation.py
+-rw-r--r--   0     1001     1002    35202 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_question.py
+-rw-r--r--   0     1001     1002    32455 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_question_base.py
+-rw-r--r--   0     1001     1002    30352 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_question_id.py
+-rw-r--r--   0     1001     1002    33478 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_question_inner.py
+-rw-r--r--   0     1001     1002    31198 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py
+-rw-r--r--   0     1001     1002    33674 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py
+-rw-r--r--   0     1001     1002    31111 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py
+-rw-r--r--   0     1001     1002    31041 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py
+-rw-r--r--   0     1001     1002    30315 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_with_exp.py
+-rw-r--r--   0     1001     1002    37164 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_recognition.py
+-rw-r--r--   0     1001     1002    34456 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_recognition_base.py
+-rw-r--r--   0     1001     1002    30333 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_recognition_id.py
+-rw-r--r--   0     1001     1002    29620 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_review_status.py
+-rw-r--r--   0     1001     1002    32583 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_source_of_truth.py
+-rw-r--r--   0     1001     1002    33457 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_truth_update.py
+-rw-r--r--   0     1001     1002    33217 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/greg_truth_updates.py
+-rw-r--r--   0     1001     1002    32202 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/grxml.py
+-rw-r--r--   0     1001     1002    32302 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/grxml_all_of.py
+-rw-r--r--   0     1001     1002    30711 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/gui_input.py
+-rw-r--r--   0     1001     1002    29329 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/hangup.py
+-rw-r--r--   0     1001     1002    30001 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/html_checkbox.py
+-rw-r--r--   0     1001     1002    31815 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/html_choice_item.py
+-rw-r--r--   0     1001     1002    30033 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/html_radio_buttons.py
+-rw-r--r--   0     1001     1002    30096 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/html_text_entry.py
+-rw-r--r--   0     1001     1002    29489 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/if_exists.py
+-rw-r--r--   0     1001     1002    33513 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/incident.py
+-rw-r--r--   0     1001     1002    30020 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/inline_data.py
+-rw-r--r--   0     1001     1002    31225 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/inline_object.py
+-rw-r--r--   0     1001     1002    31237 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/inline_object1.py
+-rw-r--r--   0     1001     1002    34640 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/input.py
+-rw-r--r--   0     1001     1002    34780 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/input_all_of.py
+-rw-r--r--   0     1001     1002    30940 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/integration.py
+-rw-r--r--   0     1001     1002    36116 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/jjsgf.py
+-rw-r--r--   0     1001     1002    36256 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/jjsgf_all_of.py
+-rw-r--r--   0     1001     1002    31407 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/keyword_spot_example.py
+-rw-r--r--   0     1001     1002    31392 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/keyword_spot_group.py
+-rw-r--r--   0     1001     1002    33135 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/keyword_spot_item.py
+-rw-r--r--   0     1001     1002    29613 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/lang_model_status.py
+-rw-r--r--   0     1001     1002    30389 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/language.py
+-rw-r--r--   0     1001     1002    39716 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/language_model_doc.py
+-rw-r--r--   0     1001     1002    38173 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/language_model_doc_modifiable.py
+-rw-r--r--   0     1001     1002    32931 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/language_model_src_data.py
+-rw-r--r--   0     1001     1002    29490 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/lm_type.py
+-rw-r--r--   0     1001     1002    30152 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/min_max_speakers.py
+-rw-r--r--   0     1001     1002    32993 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/min_max_speakers_diarization.py
+-rw-r--r--   0     1001     1002    29642 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/mood_type.py
+-rw-r--r--   0     1001     1002    31485 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/mrc_pv1_asr_settings.py
+-rw-r--r--   0     1001     1002    31458 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/mrc_pv2_asr_settings.py
+-rw-r--r--   0     1001     1002    29489 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/mrcp_version.py
+-rw-r--r--   0     1001     1002    33330 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/multipart_form_data_field.py
+-rw-r--r--   0     1001     1002    31972 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/name_value_pair.py
+-rw-r--r--   0     1001     1002    30984 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/named_entity_concept.py
+-rw-r--r--   0     1001     1002    30105 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/named_entity_type.py
+-rw-r--r--   0     1001     1002    49869 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/new_speech_analytics_session.py
+-rw-r--r--   0     1001     1002    38283 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/new_speech_analytics_session_response.py
+-rw-r--r--   0     1001     1002    30316 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/new_speech_analytics_session_response_poll.py
+-rw-r--r--   0     1001     1002    30222 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/new_speech_analytics_session_response_websocket.py
+-rw-r--r--   0     1001     1002    30870 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/non_session_error_response.py
+-rw-r--r--   0     1001     1002    29409 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/non_session_error_response400.py
+-rw-r--r--   0     1001     1002    29409 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/non_session_error_response401.py
+-rw-r--r--   0     1001     1002    32303 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/output.py
+-rw-r--r--   0     1001     1002    32383 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/output_all_of.py
+-rw-r--r--   0     1001     1002    34585 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/overtalk.py
+-rw-r--r--   0     1001     1002    32777 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/phone_audio_input.py
+-rw-r--r--   0     1001     1002    30995 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/phone_audio_input_prompt.py
+-rw-r--r--   0     1001     1002    33626 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_example.py
+-rw-r--r--   0     1001     1002    33492 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_group.py
+-rw-r--r--   0     1001     1002    41135 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_item.py
+-rw-r--r--   0     1001     1002    32456 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_item_location.py
+-rw-r--r--   0     1001     1002    32236 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_item_location_dialogue.py
+-rw-r--r--   0     1001     1002    31096 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_item_slots.py
+-rw-r--r--   0     1001     1002    33032 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/pii_redaction_conf.py
+-rw-r--r--   0     1001     1002    33834 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/poll_req.py
+-rw-r--r--   0     1001     1002    33610 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/poll_resp.py
+-rw-r--r--   0     1001     1002    33580 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/portal_output_init.py
+-rw-r--r--   0     1001     1002    30369 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/pre_fetch.py
+-rw-r--r--   0     1001     1002    41038 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/progress.py
+-rw-r--r--   0     1001     1002    31854 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/progress_callback.py
+-rw-r--r--   0     1001     1002    29776 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/progress_phase.py
+-rw-r--r--   0     1001     1002    32898 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/quartiles_energy.py
+-rw-r--r--   0     1001     1002    32874 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/quartiles_pitch.py
+-rw-r--r--   0     1001     1002    34683 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/reco_alt.py
+-rw-r--r--   0     1001     1002    31884 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/recog_nlsml.py
+-rw-r--r--   0     1001     1002    31054 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/recog_nlsml_no_exp.py
+-rw-r--r--   0     1001     1002    34148 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/recog_obj.py
+-rw-r--r--   0     1001     1002    33386 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/recog_obj_no_exp.py
+-rw-r--r--   0     1001     1002    34047 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/recognition_result.py
+-rw-r--r--   0     1001     1002    34316 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/requested_content.py
+-rw-r--r--   0     1001     1002    33327 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/resource_uri.py
+-rw-r--r--   0     1001     1002    29579 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/results_websocket_mode.py
+-rw-r--r--   0     1001     1002    35226 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/s3.py
+-rw-r--r--   0     1001     1002    35386 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/s3_all_of.py
+-rw-r--r--   0     1001     1002    35343 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/s3_audio_input.py
+-rw-r--r--   0     1001     1002    31594 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/s3_metadata_mapping.py
+-rw-r--r--   0     1001     1002    31372 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/s3_tag_mapping.py
+-rw-r--r--   0     1001     1002    29506 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sa_conf_type.py
+-rw-r--r--   0     1001     1002    29625 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sample_rate.py
+-rw-r--r--   0     1001     1002    35577 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sentence_hypothesis_or_recognition.py
+-rw-r--r--   0     1001     1002    31912 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sentence_hypothesis_or_recognition_alternatives.py
+-rw-r--r--   0     1001     1002    34034 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sentence_recognition.py
+-rw-r--r--   0     1001     1002    30202 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/session_content.py
+-rw-r--r--   0     1001     1002    31714 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/session_error_response.py
+-rw-r--r--   0     1001     1002    37730 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/session_init_recognition.py
+-rw-r--r--   0     1001     1002    39972 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/session_init_transcription.py
+-rw-r--r--   0     1001     1002    33134 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/session_init_transcription_diarization.py
+-rw-r--r--   0     1001     1002    30936 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/session_success_response.py
+-rw-r--r--   0     1001     1002    35545 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/settings_async_transcription.py
+-rw-r--r--   0     1001     1002    32466 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/settings_recognition.py
+-rw-r--r--   0     1001     1002    32439 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/settings_sync_transcription.py
+-rw-r--r--   0     1001     1002    34451 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/silence.py
+-rw-r--r--   0     1001     1002    31097 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/slot_entity.py
+-rw-r--r--   0     1001     1002    31044 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/slot_keyword.py
+-rw-r--r--   0     1001     1002    31131 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sos_ref.py
+-rw-r--r--   0     1001     1002    33790 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speaker_result.py
+-rw-r--r--   0     1001     1002    44598 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_base_result.py
+-rw-r--r--   0     1001     1002    32273 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_channel.py
+-rw-r--r--   0     1001     1002    45971 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_channel_result.py
+-rw-r--r--   0     1001     1002    34257 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_channel_with_transcribe.py
+-rw-r--r--   0     1001     1002    71029 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config.py
+-rw-r--r--   0     1001     1002    34715 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_identifying.py
+-rw-r--r--   0     1001     1002    68304 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_modifiable.py
+-rw-r--r--   0     1001     1002    67024 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_modifiable_base.py
+-rw-r--r--   0     1001     1002    31582 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py
+-rw-r--r--   0     1001     1002    31125 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_name_optional.py
+-rw-r--r--   0     1001     1002    31279 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_name_required.py
+-rw-r--r--   0     1001     1002    50325 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_core_result.py
+-rw-r--r--   0     1001     1002    35252 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_core_result_all_of.py
+-rw-r--r--   0     1001     1002    31191 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_criteria_data.py
+-rw-r--r--   0     1001     1002    31656 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_emotion.py
+-rw-r--r--   0     1001     1002    30859 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_emotion_data.py
+-rw-r--r--   0     1001     1002    36980 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_emotion_item.py
+-rw-r--r--   0     1001     1002    30905 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword.py
+-rw-r--r--   0     1001     1002    31195 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword_data.py
+-rw-r--r--   0     1001     1002    36229 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword_item.py
+-rw-r--r--   0     1001     1002    36481 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py
+-rw-r--r--   0     1001     1002    32743 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py
+-rw-r--r--   0     1001     1002    31875 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_named_entity.py
+-rw-r--r--   0     1001     1002    37279 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_named_entity_item.py
+-rw-r--r--   0     1001     1002    37567 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py
+-rw-r--r--   0     1001     1002    33817 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py
+-rw-r--r--   0     1001     1002    32961 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase.py
+-rw-r--r--   0     1001     1002    31178 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_data.py
+-rw-r--r--   0     1001     1002    33076 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_for_ws.py
+-rw-r--r--   0     1001     1002    31165 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py
+-rw-r--r--   0     1001     1002    31004 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_group.py
+-rw-r--r--   0     1001     1002    31277 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_group_data.py
+-rw-r--r--   0     1001     1002    31037 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py
+-rw-r--r--   0     1001     1002    36392 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_group_item.py
+-rw-r--r--   0     1001     1002    38301 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_item.py
+-rw-r--r--   0     1001     1002    39701 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py
+-rw-r--r--   0     1001     1002    31075 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_slots.py
+-rw-r--r--   0     1001     1002    61305 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_result.py
+-rw-r--r--   0     1001     1002    46632 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_result_detail.py
+-rw-r--r--   0     1001     1002    31090 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_session_modifiable.py
+-rw-r--r--   0     1001     1002    38025 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_session_poll_response.py
+-rw-r--r--   0     1001     1002    36320 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_websocket_payload.py
+-rw-r--r--   0     1001     1002    31727 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/start_end_time_for_sub_criterion.py
+-rw-r--r--   0     1001     1002    30413 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/stomp_ping.py
+-rw-r--r--   0     1001     1002    33033 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/stomp_word_correction.py
+-rw-r--r--   0     1001     1002    37052 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/stomp_ws_word.py
+-rw-r--r--   0     1001     1002    31190 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/stomp_ws_word_all_of.py
+-rw-r--r--   0     1001     1002    35347 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/stomp_ws_word_base.py
+-rw-r--r--   0     1001     1002    35619 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/stream_resp.py
+-rw-r--r--   0     1001     1002    33180 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/stream_setup.py
+-rw-r--r--   0     1001     1002    29633 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/streaming_protocol.py
+-rw-r--r--   0     1001     1002    38812 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sub_criterion_config.py
+-rw-r--r--   0     1001     1002    41198 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sub_criterion_satisfied.py
+-rw-r--r--   0     1001     1002    32173 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sync_audio_input_source.py
+-rw-r--r--   0     1001     1002    31121 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sync_recognition_request.py
+-rw-r--r--   0     1001     1002    32686 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sync_recognition_response.py
+-rw-r--r--   0     1001     1002    30289 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sync_session_established.py
+-rw-r--r--   0     1001     1002    31005 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sync_transcription_request.py
+-rw-r--r--   0     1001     1002    32744 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sync_transcription_response.py
+-rw-r--r--   0     1001     1002    33183 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/sync_transcription_result.py
+-rw-r--r--   0     1001     1002    38899 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/talk_time.py
+-rw-r--r--   0     1001     1002    31430 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/topic_score.py
+-rw-r--r--   0     1001     1002    29529 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_bucket_type.py
+-rw-r--r--   0     1001     1002    39171 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_doc.py
+-rw-r--r--   0     1001     1002    31089 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_doc_defaults.py
+-rw-r--r--   0     1001     1002    36549 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_doc_statistics.py
+-rw-r--r--   0     1001     1002    34623 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_key.py
+-rw-r--r--   0     1001     1002    33873 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_modifiable.py
+-rw-r--r--   0     1001     1002    29621 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_status.py
+-rw-r--r--   0     1001     1002    29661 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_status_modifiable.py
+-rw-r--r--   0     1001     1002    29549 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/training_set_store_type.py
+-rw-r--r--   0     1001     1002    31791 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transcribe_alt.py
+-rw-r--r--   0     1001     1002    31073 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transcribe_session_id.py
+-rw-r--r--   0     1001     1002    34091 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transcribe_session_modify_request.py
+-rw-r--r--   0     1001     1002    31768 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transcribe_session_modify_request_mute.py
+-rw-r--r--   0     1001     1002    30596 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transcribe_session_modify_request_pause.py
+-rw-r--r--   0     1001     1002    34625 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transcript_position_range.py
+-rw-r--r--   0     1001     1002    34805 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transcript_position_range_for_phrase.py
+-rw-r--r--   0     1001     1002    36041 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py
+-rw-r--r--   0     1001     1002    36362 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transfer.py
+-rw-r--r--   0     1001     1002    36502 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/transfer_all_of.py
+-rw-r--r--   0     1001     1002    29545 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/vad_mode.py
+-rw-r--r--   0     1001     1002    32350 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/version.py
+-rw-r--r--   0     1001     1002    38002 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/websocket.py
+-rw-r--r--   0     1001     1002    41056 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/websocket_init.py
+-rw-r--r--   0     1001     1002    30563 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/websocket_init_reco.py
+-rw-r--r--   0     1001     1002    36158 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/websocket_modifiable.py
+-rw-r--r--   0     1001     1002    32626 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/websocket_msg.py
+-rw-r--r--   0     1001     1002    29492 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/websocket_protocol.py
+-rw-r--r--   0     1001     1002    30967 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/websocket_resp.py
+-rw-r--r--   0     1001     1002    30324 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/word_alternatives.py
+-rw-r--r--   0     1001     1002    31504 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/word_cloud_item.py
+-rw-r--r--   0     1001     1002    31345 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/word_correction.py
+-rw-r--r--   0     1001     1002    36355 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/word_item_timed.py
+-rw-r--r--   0     1001     1002    31430 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/word_item_timing.py
+-rw-r--r--   0     1001     1002    30685 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/word_tree_ids.py
+-rw-r--r--   0     1001     1002    36732 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/word_tree_item.py
+-rw-r--r--   0     1001     1002    33287 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/words_item.py
+-rw-r--r--   0     1001     1002    36590 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/words_section.py
+-rw-r--r--   0     1001     1002    33136 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/words_section_meta.py
+-rw-r--r--   0     1001     1002    32138 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/words_section_meta_mc.py
+-rw-r--r--   0     1001     1002    34117 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/words_section_single_column.py
+-rw-r--r--   0     1001     1002    30198 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/words_section_words.py
+-rw-r--r--   0     1001     1002    44223 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/words_websocket_item.py
+-rw-r--r--   0     1001     1002    33874 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_emotion_item.py
+-rw-r--r--   0     1001     1002    33123 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_keyword_item.py
+-rw-r--r--   0     1001     1002    34113 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_named_entity_item.py
+-rw-r--r--   0     1001     1002    32347 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_phrase_group_item.py
+-rw-r--r--   0     1001     1002    35126 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_phrase_item.py
+-rw-r--r--   0     1001     1002    35478 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_phrase_item_inside_group.py
+-rw-r--r--   0     1001     1002    31699 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_position_range.py
+-rw-r--r--   0     1001     1002    30883 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_position_range_nested.py
+-rw-r--r--   0     1001     1002    30871 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_position_range_no_spk.py
+-rw-r--r--   0     1001     1002    37496 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py
+-rw-r--r--   0     1001     1002    31348 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py
+-rw-r--r--   0     1001     1002    32681 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_speaker.py
+-rw-r--r--   0     1001     1002    34541 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_word.py
+-rw-r--r--   0     1001     1002    32107 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/models/ws_word_edit.py
+-rw-r--r--   0     1001     1002    39168 2023-06-07 19:40:00.000000 voicegain-speech-1.84.1/voicegain_speech/rest.py
+drwxr-xr-x   0     1001     1002        0 2023-06-07 19:40:03.597644 voicegain-speech-1.84.1/voicegain_speech.egg-info/
+-rw-r--r--   0     1001     1002     2923 2023-06-07 19:40:03.000000 voicegain-speech-1.84.1/voicegain_speech.egg-info/PKG-INFO
+-rw-r--r--   0     1001     1002    22939 2023-06-07 19:40:03.000000 voicegain-speech-1.84.1/voicegain_speech.egg-info/SOURCES.txt
+-rw-r--r--   0     1001     1002        1 2023-06-07 19:40:03.000000 voicegain-speech-1.84.1/voicegain_speech.egg-info/dependency_links.txt
+-rw-r--r--   0     1001     1002       48 2023-06-07 19:40:03.000000 voicegain-speech-1.84.1/voicegain_speech.egg-info/requires.txt
+-rw-r--r--   0     1001     1002       17 2023-06-07 19:40:03.000000 voicegain-speech-1.84.1/voicegain_speech.egg-info/top_level.txt
```

### Comparing `voicegain-speech-1.84.0/LICENSE` & `voicegain-speech-1.84.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/PKG-INFO` & `voicegain-speech-1.84.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: voicegain-speech
-Version: 1.84.0
+Version: 1.84.1
 Summary: Voicegain Speech-to-Text Python SDK
 Home-page: UNKNOWN
 Author: Huishen Zhan, Kuo Zhang, Jacek Jarmulak
 Author-email: huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai
 License: UNKNOWN
-Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.84.0.tar.gz
+Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.84.1.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Voicegain Speech-to-Text Python SDK
 
 Python SDK for the [Voicegain](https://www.voicegain.ai) [Speech-to-Text API](https://portal.voicegain.ai/api/v1/index.html).
```

### Comparing `voicegain-speech-1.84.0/README.md` & `voicegain-speech-1.84.1/README.md`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/setup.py` & `voicegain-speech-1.84.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="voicegain-speech",
-    version="1.84.0",
+    version="1.84.1",
     author="Huishen Zhan, Kuo Zhang, Jacek Jarmulak",
     author_email="huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai",
     description="Voicegain Speech-to-Text Python SDK",
-    download_url='https://github.com/voicegain/python-sdk/archive/refs/tags/1.84.0.tar.gz',
+    download_url='https://github.com/voicegain/python-sdk/archive/refs/tags/1.84.1.tar.gz',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=REQUIRES,
     packages=setuptools.find_packages(),
     include_package_data=True,
 )
```

### Comparing `voicegain-speech-1.84.0/voicegain_speech/__init__.py` & `voicegain-speech-1.84.1/voicegain_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/__init__.py` & `voicegain-speech-1.84.1/voicegain_speech/api/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/aivr_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/aivr_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/aivr_callback_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/aivr_callback_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/asr_callback_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/asr_callback_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/audiocodes_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/audiocodes_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/data_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/data_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/greg_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/greg_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/lm_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/lm_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/recognize_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/recognize_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/sa_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/sa_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/security_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/security_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/training_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/training_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/transcribe_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/transcribe_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api/websocket_api.py` & `voicegain-speech-1.84.1/voicegain_speech/api/websocket_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/api_client.py` & `voicegain-speech-1.84.1/voicegain_speech/api_client.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/configuration.py` & `voicegain-speech-1.84.1/voicegain_speech/configuration.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/exceptions.py` & `voicegain-speech-1.84.1/voicegain_speech/exceptions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/__init__.py` & `voicegain-speech-1.84.1/voicegain_speech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_control_messages.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_control_messages.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_end.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_end.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_error.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_error.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_hypothesis.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_hypothesis.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_hypothesis_alternatives.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_hypothesis_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_recognition_alternatives.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_recognition_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_response_messages.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_response_messages.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_start.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_start.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_start_stt_speech_contexts.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_start_stt_speech_contexts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_started.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_started.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ac_stop.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ac_stop.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/account_and_context_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/account_and_context_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/advanced_regex.py` & `voicegain-speech-1.84.1/voicegain_speech/models/advanced_regex.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aircall.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aircall.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aircall_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aircall_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_callback_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_callback_response_final.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_callback_response_final.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_conference_transfer.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_conference_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_disconnect.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_disconnect.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_event.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_event_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_event_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_existing_session.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_existing_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_logic.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_logic.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_logic_media.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_logic_media.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_logic_transfer.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_logic_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_logic_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_logic_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_new_session.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_new_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_phone_transfer.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_phone_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt_completion.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt_completion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt_playing.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt_playing.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt_properties_audio.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt_properties_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_prompt_properties_html.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_prompt_properties_html.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_question.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_question.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_recognition_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_recording.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_recording.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_response_properties_audio.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_response_properties_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_response_properties_html.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_response_properties_html.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_session_user.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_session_user.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_session_user_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_session_user_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_session_user_fs.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_session_user_fs.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivr_transfer.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivr_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/aivrs_question_specifics.py` & `voicegain-speech-1.84.1/voicegain_speech/models/aivrs_question_specifics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/answer_map_entry.py` & `voicegain-speech-1.84.1/voicegain_speech/models/answer_map_entry.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_event.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_status.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_status_additional.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_status_additional.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_status_after_input_started.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_status_after_input_started.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_processing_status_for_callback.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_processing_status_for_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_recognition_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_common.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_common.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_recognition_defaults.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_recognition_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_recognition_grammars_etc.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_recognition_grammars_etc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_recognition_timeouts.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_recognition_timeouts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_async.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_async_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_async_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_common.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_common.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_common_lm.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_common_lm.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_default_timeouts.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_default_timeouts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_defaults.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_sa.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_sa.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_speakers.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_speakers.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/asr_transcribe_queue_status.py` & `voicegain-speech-1.84.1/voicegain_speech/models/asr_transcribe_queue_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_audio_input_source.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_audio_input_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_mode.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_mode_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_mode_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_mode_speech_analytics.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_mode_speech_analytics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_mode_transcription.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_mode_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_post_response_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_post_response_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_post_response_base_audio.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_post_response_base_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_reco_post_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_reco_post_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_reco_post_response_sessions.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_reco_post_response_sessions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_callback_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_request.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_recognition_result_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_recognition_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_full.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_full.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_audio.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_audio_callback.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_audio_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_audio_source.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_audio_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_full_all_of_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_full_all_of_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental_detail.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental_detail.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental_detail_control_status.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental_detail_control_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental_detail_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental_detail_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_session_established.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_session_short_info.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_session_short_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_session_url.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_session_url.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_transc_post_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_transc_post_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_transc_post_response_sessions.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_transc_post_response_sessions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_transc_session_established.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_transc_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_transcription_callback_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_transcription_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_transcription_request.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_transcription_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_transcription_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_transcription_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/async_transcription_response_shared.py` & `voicegain-speech-1.84.1/voicegain_speech/models/async_transcription_response_shared.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_channel.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_channel.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_channel_selector.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_channel_selector.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_channel_selector_offline_async.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_channel_selector_offline_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_channels.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_channels.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_for_data_object.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_for_data_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_format.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_format.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_async.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_async_source.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_async_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_async_with_callback.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_async_with_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_callback.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_callback_callback.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_callback_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_data_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_data_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_data_all_of_source.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_data_all_of_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_sync.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_sync.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_input_sync_source.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_input_sync_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_resource_uri.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_resource_uri.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_zone_class.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_zone_class.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/audio_zone_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/audio_zone_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/basic_success_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/basic_success_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/builtin.py` & `voicegain-speech-1.84.1/voicegain_speech/models/builtin.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/builtin_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/builtin_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/call_attributes.py` & `voicegain-speech-1.84.1/voicegain_speech/models/call_attributes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/call_review_answer_alone.py` & `voicegain-speech-1.84.1/voicegain_speech/models/call_review_answer_alone.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/call_review_answer_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/call_review_answer_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/call_review_config_question_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/call_review_config_question_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/call_review_config_question_base_with_answer.py` & `voicegain-speech-1.84.1/voicegain_speech/models/call_review_config_question_base_with_answer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/call_review_config_question_base_with_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/call_review_config_question_base_with_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/callback_req.py` & `voicegain-speech-1.84.1/voicegain_speech/models/callback_req.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/callback_req_reco.py` & `voicegain-speech-1.84.1/voicegain_speech/models/callback_req_reco.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/callback_resp.py` & `voicegain-speech-1.84.1/voicegain_speech/models/callback_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/caption.py` & `voicegain-speech-1.84.1/voicegain_speech/models/caption.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/compliance_settings.py` & `voicegain-speech-1.84.1/voicegain_speech/models/compliance_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/config_value_status.py` & `voicegain-speech-1.84.1/voicegain_speech/models/config_value_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/content_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/content_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/continuous_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/continuous_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/core_aivr_session.py` & `voicegain-speech-1.84.1/voicegain_speech/models/core_aivr_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/core_aivr_session_telco_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/core_aivr_session_telco_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/cr_question_id_for_cr_config.py` & `voicegain-speech-1.84.1/voicegain_speech/models/cr_question_id_for_cr_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/creating_entity.py` & `voicegain-speech-1.84.1/voicegain_speech/models/creating_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/criterion_config.py` & `voicegain-speech-1.84.1/voicegain_speech/models/criterion_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/criterion_satisfied.py` & `voicegain-speech-1.84.1/voicegain_speech/models/criterion_satisfied.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/data_obj_ref.py` & `voicegain-speech-1.84.1/voicegain_speech/models/data_obj_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/data_object.py` & `voicegain-speech-1.84.1/voicegain_speech/models/data_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/data_object_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/data_object_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/data_object_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/data_object_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/data_object_ids.py` & `voicegain-speech-1.84.1/voicegain_speech/models/data_object_ids.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/data_object_no_sos_ref.py` & `voicegain-speech-1.84.1/voicegain_speech/models/data_object_no_sos_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/data_object_with_audio.py` & `voicegain-speech-1.84.1/voicegain_speech/models/data_object_with_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/debug_info.py` & `voicegain-speech-1.84.1/voicegain_speech/models/debug_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/debug_settings.py` & `voicegain-speech-1.84.1/voicegain_speech/models/debug_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/demo.py` & `voicegain-speech-1.84.1/voicegain_speech/models/demo.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/demo_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/demo_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/diarization_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/diarization_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/diarization_zone.py` & `voicegain-speech-1.84.1/voicegain_speech/models/diarization_zone.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/diarization_zone_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/diarization_zone_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/disconnect.py` & `voicegain-speech-1.84.1/voicegain_speech/models/disconnect.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/disconnect_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/disconnect_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/error.py` & `voicegain-speech-1.84.1/voicegain_speech/models/error.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/error_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/error_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/error_info.py` & `voicegain-speech-1.84.1/voicegain_speech/models/error_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/estimated_queue_wait.py` & `voicegain-speech-1.84.1/voicegain_speech/models/estimated_queue_wait.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/experiment_platform.py` & `voicegain-speech-1.84.1/voicegain_speech/models/experiment_platform.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/file_location.py` & `voicegain-speech-1.84.1/voicegain_speech/models/file_location.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/formatter.py` & `voicegain-speech-1.84.1/voicegain_speech/models/formatter.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/grammar.py` & `voicegain-speech-1.84.1/voicegain_speech/models/grammar.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_base_with_audio.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_base_with_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_input.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_input_audio_hash.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_input_audio_hash.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_input_audio_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_input_audio_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_input_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_input_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_base_inclusive.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_base_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_core.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_inclusive.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_inclusive_core.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_inclusive_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_inner.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_set_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_set_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_audio_thin.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_audio_thin.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_base_inclusive.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_base_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_base_platform_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_base_platform_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_inclusive.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_modifiable.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_platform_external_asr.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_platform_external_asr.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_platform_upload.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_platform_upload.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_platform_voicegain.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_platform_voicegain.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_status.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_experiment_status_modifiable.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_experiment_status_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_base_light.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_base_light.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_inner.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_grammar_light.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_grammar_light.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_interpretation.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_interpretation.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_question.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_question.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_question_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_question_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_question_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_question_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_question_inner.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_question_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_recog_base_with_exp.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_recog_base_with_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_recognition_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_recognition_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_recognition_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_recognition_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_review_status.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_review_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_source_of_truth.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_source_of_truth.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_truth_update.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_truth_update.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/greg_truth_updates.py` & `voicegain-speech-1.84.1/voicegain_speech/models/greg_truth_updates.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/grxml.py` & `voicegain-speech-1.84.1/voicegain_speech/models/grxml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/grxml_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/grxml_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/gui_input.py` & `voicegain-speech-1.84.1/voicegain_speech/models/gui_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/hangup.py` & `voicegain-speech-1.84.1/voicegain_speech/models/hangup.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/html_checkbox.py` & `voicegain-speech-1.84.1/voicegain_speech/models/html_checkbox.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/html_choice_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/html_choice_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/html_radio_buttons.py` & `voicegain-speech-1.84.1/voicegain_speech/models/html_radio_buttons.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/html_text_entry.py` & `voicegain-speech-1.84.1/voicegain_speech/models/html_text_entry.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/if_exists.py` & `voicegain-speech-1.84.1/voicegain_speech/models/if_exists.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/incident.py` & `voicegain-speech-1.84.1/voicegain_speech/models/incident.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/inline_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/inline_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/inline_object.py` & `voicegain-speech-1.84.1/voicegain_speech/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/inline_object1.py` & `voicegain-speech-1.84.1/voicegain_speech/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/input.py` & `voicegain-speech-1.84.1/voicegain_speech/models/input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/input_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/input_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/integration.py` & `voicegain-speech-1.84.1/voicegain_speech/models/integration.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/jjsgf.py` & `voicegain-speech-1.84.1/voicegain_speech/models/jjsgf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/jjsgf_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/jjsgf_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/keyword_spot_example.py` & `voicegain-speech-1.84.1/voicegain_speech/models/keyword_spot_example.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/keyword_spot_group.py` & `voicegain-speech-1.84.1/voicegain_speech/models/keyword_spot_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/keyword_spot_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/keyword_spot_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/lang_model_status.py` & `voicegain-speech-1.84.1/voicegain_speech/models/lang_model_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/language.py` & `voicegain-speech-1.84.1/voicegain_speech/models/language.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/language_model_doc.py` & `voicegain-speech-1.84.1/voicegain_speech/models/language_model_doc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/language_model_doc_modifiable.py` & `voicegain-speech-1.84.1/voicegain_speech/models/language_model_doc_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/language_model_src_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/language_model_src_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/lm_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/lm_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/min_max_speakers.py` & `voicegain-speech-1.84.1/voicegain_speech/models/min_max_speakers.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/min_max_speakers_diarization.py` & `voicegain-speech-1.84.1/voicegain_speech/models/min_max_speakers_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/mood_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/mood_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/mrc_pv1_asr_settings.py` & `voicegain-speech-1.84.1/voicegain_speech/models/mrc_pv1_asr_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/mrc_pv2_asr_settings.py` & `voicegain-speech-1.84.1/voicegain_speech/models/mrc_pv2_asr_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/mrcp_version.py` & `voicegain-speech-1.84.1/voicegain_speech/models/mrcp_version.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/multipart_form_data_field.py` & `voicegain-speech-1.84.1/voicegain_speech/models/multipart_form_data_field.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/name_value_pair.py` & `voicegain-speech-1.84.1/voicegain_speech/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/named_entity_concept.py` & `voicegain-speech-1.84.1/voicegain_speech/models/named_entity_concept.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/named_entity_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/named_entity_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/new_speech_analytics_session.py` & `voicegain-speech-1.84.1/voicegain_speech/models/new_speech_analytics_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/new_speech_analytics_session_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/new_speech_analytics_session_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/new_speech_analytics_session_response_poll.py` & `voicegain-speech-1.84.1/voicegain_speech/models/new_speech_analytics_session_response_poll.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/new_speech_analytics_session_response_websocket.py` & `voicegain-speech-1.84.1/voicegain_speech/models/new_speech_analytics_session_response_websocket.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/non_session_error_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/non_session_error_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/non_session_error_response400.py` & `voicegain-speech-1.84.1/voicegain_speech/models/non_session_error_response400.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/non_session_error_response401.py` & `voicegain-speech-1.84.1/voicegain_speech/models/non_session_error_response401.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/output.py` & `voicegain-speech-1.84.1/voicegain_speech/models/output.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/output_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/output_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/overtalk.py` & `voicegain-speech-1.84.1/voicegain_speech/models/overtalk.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/phone_audio_input.py` & `voicegain-speech-1.84.1/voicegain_speech/models/phone_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/phone_audio_input_prompt.py` & `voicegain-speech-1.84.1/voicegain_speech/models/phone_audio_input_prompt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_example.py` & `voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_example.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_group.py` & `voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_item_location.py` & `voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_item_location.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_item_location_dialogue.py` & `voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_item_location_dialogue.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/phrase_spot_item_slots.py` & `voicegain-speech-1.84.1/voicegain_speech/models/phrase_spot_item_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/pii_redaction_conf.py` & `voicegain-speech-1.84.1/voicegain_speech/models/pii_redaction_conf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/poll_req.py` & `voicegain-speech-1.84.1/voicegain_speech/models/poll_req.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/poll_resp.py` & `voicegain-speech-1.84.1/voicegain_speech/models/poll_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/portal_output_init.py` & `voicegain-speech-1.84.1/voicegain_speech/models/portal_output_init.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/pre_fetch.py` & `voicegain-speech-1.84.1/voicegain_speech/models/pre_fetch.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/progress.py` & `voicegain-speech-1.84.1/voicegain_speech/models/progress.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/progress_callback.py` & `voicegain-speech-1.84.1/voicegain_speech/models/progress_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/progress_phase.py` & `voicegain-speech-1.84.1/voicegain_speech/models/progress_phase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/quartiles_energy.py` & `voicegain-speech-1.84.1/voicegain_speech/models/quartiles_energy.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/quartiles_pitch.py` & `voicegain-speech-1.84.1/voicegain_speech/models/quartiles_pitch.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/reco_alt.py` & `voicegain-speech-1.84.1/voicegain_speech/models/reco_alt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/recog_nlsml.py` & `voicegain-speech-1.84.1/voicegain_speech/models/recog_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/recog_nlsml_no_exp.py` & `voicegain-speech-1.84.1/voicegain_speech/models/recog_nlsml_no_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/recog_obj.py` & `voicegain-speech-1.84.1/voicegain_speech/models/recog_obj.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/recog_obj_no_exp.py` & `voicegain-speech-1.84.1/voicegain_speech/models/recog_obj_no_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/recognition_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/requested_content.py` & `voicegain-speech-1.84.1/voicegain_speech/models/requested_content.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/resource_uri.py` & `voicegain-speech-1.84.1/voicegain_speech/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/results_websocket_mode.py` & `voicegain-speech-1.84.1/voicegain_speech/models/results_websocket_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/s3.py` & `voicegain-speech-1.84.1/voicegain_speech/models/s3.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/s3_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/s3_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/s3_audio_input.py` & `voicegain-speech-1.84.1/voicegain_speech/models/s3_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/s3_metadata_mapping.py` & `voicegain-speech-1.84.1/voicegain_speech/models/s3_metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/s3_tag_mapping.py` & `voicegain-speech-1.84.1/voicegain_speech/models/s3_tag_mapping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sa_conf_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sa_conf_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sample_rate.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sample_rate.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sentence_hypothesis_or_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sentence_hypothesis_or_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sentence_hypothesis_or_recognition_alternatives.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sentence_hypothesis_or_recognition_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sentence_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sentence_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/session_content.py` & `voicegain-speech-1.84.1/voicegain_speech/models/session_content.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/session_error_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/session_error_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/session_init_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/session_init_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/session_init_transcription.py` & `voicegain-speech-1.84.1/voicegain_speech/models/session_init_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/session_init_transcription_diarization.py` & `voicegain-speech-1.84.1/voicegain_speech/models/session_init_transcription_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/session_success_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/session_success_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/settings_async_transcription.py` & `voicegain-speech-1.84.1/voicegain_speech/models/settings_async_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/settings_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/settings_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/settings_sync_transcription.py` & `voicegain-speech-1.84.1/voicegain_speech/models/settings_sync_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/silence.py` & `voicegain-speech-1.84.1/voicegain_speech/models/silence.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/slot_entity.py` & `voicegain-speech-1.84.1/voicegain_speech/models/slot_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/slot_keyword.py` & `voicegain-speech-1.84.1/voicegain_speech/models/slot_keyword.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sos_ref.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sos_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speaker_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speaker_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_base_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_base_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_channel.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_channel.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_channel_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_channel_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_channel_with_transcribe.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_channel_with_transcribe.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_identifying.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_identifying.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_modifiable.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_modifiable_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_modifiable_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_name_optional.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_name_optional.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_config_name_required.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_config_name_required.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_core_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_core_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_core_result_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_core_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_criteria_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_criteria_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_emotion.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_emotion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_emotion_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_emotion_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_emotion_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_emotion_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_named_entity.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_named_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_named_entity_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_named_entity_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_for_ws.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_group.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_group_data.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_group_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_group_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_group_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_phrase_slots.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_phrase_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_result_detail.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_result_detail.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_session_modifiable.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_session_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_session_poll_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_session_poll_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/speech_analytics_websocket_payload.py` & `voicegain-speech-1.84.1/voicegain_speech/models/speech_analytics_websocket_payload.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/start_end_time_for_sub_criterion.py` & `voicegain-speech-1.84.1/voicegain_speech/models/start_end_time_for_sub_criterion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/stomp_ping.py` & `voicegain-speech-1.84.1/voicegain_speech/models/stomp_ping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/stomp_word_correction.py` & `voicegain-speech-1.84.1/voicegain_speech/models/stomp_word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/stomp_ws_word.py` & `voicegain-speech-1.84.1/voicegain_speech/models/stomp_ws_word.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/stomp_ws_word_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/stomp_ws_word_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/stomp_ws_word_base.py` & `voicegain-speech-1.84.1/voicegain_speech/models/stomp_ws_word_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/stream_resp.py` & `voicegain-speech-1.84.1/voicegain_speech/models/stream_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/stream_setup.py` & `voicegain-speech-1.84.1/voicegain_speech/models/stream_setup.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/streaming_protocol.py` & `voicegain-speech-1.84.1/voicegain_speech/models/streaming_protocol.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sub_criterion_config.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sub_criterion_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sub_criterion_satisfied.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sub_criterion_satisfied.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sync_audio_input_source.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sync_audio_input_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sync_recognition_request.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sync_recognition_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sync_recognition_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sync_recognition_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sync_session_established.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sync_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sync_transcription_request.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sync_transcription_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sync_transcription_response.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sync_transcription_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/sync_transcription_result.py` & `voicegain-speech-1.84.1/voicegain_speech/models/sync_transcription_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/talk_time.py` & `voicegain-speech-1.84.1/voicegain_speech/models/talk_time.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/topic_score.py` & `voicegain-speech-1.84.1/voicegain_speech/models/topic_score.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_bucket_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_bucket_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_doc.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_doc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_doc_defaults.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_doc_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_doc_statistics.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_doc_statistics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_key.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_key.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_modifiable.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_status.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_status_modifiable.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_status_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/training_set_store_type.py` & `voicegain-speech-1.84.1/voicegain_speech/models/training_set_store_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transcribe_alt.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transcribe_alt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transcribe_session_id.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transcribe_session_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transcribe_session_modify_request.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transcribe_session_modify_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transcribe_session_modify_request_mute.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transcribe_session_modify_request_mute.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transcribe_session_modify_request_pause.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transcribe_session_modify_request_pause.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transcript_position_range.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transcript_position_range.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transcript_position_range_for_phrase.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transcript_position_range_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transfer.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/transfer_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/transfer_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/vad_mode.py` & `voicegain-speech-1.84.1/voicegain_speech/models/vad_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/version.py` & `voicegain-speech-1.84.1/voicegain_speech/models/version.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/websocket.py` & `voicegain-speech-1.84.1/voicegain_speech/models/websocket.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/websocket_init.py` & `voicegain-speech-1.84.1/voicegain_speech/models/websocket_init.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/websocket_init_reco.py` & `voicegain-speech-1.84.1/voicegain_speech/models/websocket_init_reco.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/websocket_modifiable.py` & `voicegain-speech-1.84.1/voicegain_speech/models/websocket_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/websocket_msg.py` & `voicegain-speech-1.84.1/voicegain_speech/models/websocket_msg.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/websocket_protocol.py` & `voicegain-speech-1.84.1/voicegain_speech/models/websocket_protocol.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/websocket_resp.py` & `voicegain-speech-1.84.1/voicegain_speech/models/websocket_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/word_alternatives.py` & `voicegain-speech-1.84.1/voicegain_speech/models/word_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/word_cloud_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/word_cloud_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/word_correction.py` & `voicegain-speech-1.84.1/voicegain_speech/models/word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/word_item_timed.py` & `voicegain-speech-1.84.1/voicegain_speech/models/word_item_timed.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/word_item_timing.py` & `voicegain-speech-1.84.1/voicegain_speech/models/word_item_timing.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/word_tree_ids.py` & `voicegain-speech-1.84.1/voicegain_speech/models/word_tree_ids.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/word_tree_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/word_tree_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/words_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/words_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/words_section.py` & `voicegain-speech-1.84.1/voicegain_speech/models/words_section.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/words_section_meta.py` & `voicegain-speech-1.84.1/voicegain_speech/models/words_section_meta.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/words_section_meta_mc.py` & `voicegain-speech-1.84.1/voicegain_speech/models/words_section_meta_mc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/words_section_single_column.py` & `voicegain-speech-1.84.1/voicegain_speech/models/words_section_single_column.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/words_section_words.py` & `voicegain-speech-1.84.1/voicegain_speech/models/words_section_words.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/words_websocket_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/words_websocket_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_emotion_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_emotion_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_keyword_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_keyword_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_named_entity_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_named_entity_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_phrase_group_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_phrase_group_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_phrase_item.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_phrase_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_phrase_item_inside_group.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_phrase_item_inside_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_position_range.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_position_range.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_position_range_nested.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_position_range_nested.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sa_position_range_no_spk.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sa_position_range_no_spk.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_speaker.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_speaker.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_word.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_word.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/models/ws_word_edit.py` & `voicegain-speech-1.84.1/voicegain_speech/models/ws_word_edit.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech/rest.py` & `voicegain-speech-1.84.1/voicegain_speech/rest.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.84.0/voicegain_speech.egg-info/PKG-INFO` & `voicegain-speech-1.84.1/voicegain_speech.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: voicegain-speech
-Version: 1.84.0
+Version: 1.84.1
 Summary: Voicegain Speech-to-Text Python SDK
 Home-page: UNKNOWN
 Author: Huishen Zhan, Kuo Zhang, Jacek Jarmulak
 Author-email: huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai
 License: UNKNOWN
-Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.84.0.tar.gz
+Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.84.1.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Voicegain Speech-to-Text Python SDK
 
 Python SDK for the [Voicegain](https://www.voicegain.ai) [Speech-to-Text API](https://portal.voicegain.ai/api/v1/index.html).
```

### Comparing `voicegain-speech-1.84.0/voicegain_speech.egg-info/SOURCES.txt` & `voicegain-speech-1.84.1/voicegain_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

