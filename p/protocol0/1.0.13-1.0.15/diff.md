# Comparing `tmp/protocol0-1.0.13.tar.gz` & `tmp/protocol0-1.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protocol0-1.0.13.tar", max compression
+gzip compressed data, was "protocol0-1.0.15.tar", max compression
```

## Comparing `protocol0-1.0.13.tar` & `protocol0-1.0.15.tar`

### file list

```diff
@@ -1,552 +1,562 @@
--rw-r--r--   0        0        0     1091 2023-06-04 10:45:57.549172 protocol0-1.0.13/LICENSE.md
--rw-r--r--   0        0        0      421 2023-06-04 10:45:57.555137 protocol0-1.0.13/protocol0/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.565833 protocol0-1.0.13/protocol0/application/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.605682 protocol0-1.0.13/protocol0/application/command/__init__.py
--rw-r--r--   0        0        0      152 2023-06-04 10:45:57.567447 protocol0-1.0.13/protocol0/application/command/BounceTrackToAudioCommand.py
--rw-r--r--   0        0        0      155 2023-06-04 10:45:57.568433 protocol0-1.0.13/protocol0/application/command/CheckAudioExportValidCommand.py
--rw-r--r--   0        0        0      151 2023-06-04 10:45:57.570579 protocol0-1.0.13/protocol0/application/command/DrumRackToSimplerCommand.py
--rw-r--r--   0        0        0      356 2023-06-04 10:45:57.571591 protocol0-1.0.13/protocol0/application/command/EmitBackendEventCommand.py
--rw-r--r--   0        0        0      356 2023-06-04 10:45:57.572591 protocol0-1.0.13/protocol0/application/command/FireSceneToPositionCommand.py
--rw-r--r--   0        0        0      151 2023-06-04 10:45:57.573707 protocol0-1.0.13/protocol0/application/command/FireSelectedSceneCommand.py
--rw-r--r--   0        0        0      145 2023-06-04 10:45:57.573707 protocol0-1.0.13/protocol0/application/command/GetSetStateCommand.py
--rw-r--r--   0        0        0      148 2023-06-04 10:45:57.574719 protocol0-1.0.13/protocol0/application/command/GoToGroupTrackCommand.py
--rw-r--r--   0        0        0      288 2023-06-04 10:45:57.575761 protocol0-1.0.13/protocol0/application/command/LoadDeviceCommand.py
--rw-r--r--   0        0        0      389 2023-06-04 10:45:57.576774 protocol0-1.0.13/protocol0/application/command/LoadDrumRackCommand.py
--rw-r--r--   0        0        0      151 2023-06-04 10:45:57.577813 protocol0-1.0.13/protocol0/application/command/LoadMatchingTrackCommand.py
--rw-r--r--   0        0        0      146 2023-06-04 10:45:57.579832 protocol0-1.0.13/protocol0/application/command/LoadMinitaurCommand.py
--rw-r--r--   0        0        0      142 2023-06-04 10:45:57.580882 protocol0-1.0.13/protocol0/application/command/LoadRev2Command.py
--rw-r--r--   0        0        0      315 2023-06-04 10:45:57.581884 protocol0-1.0.13/protocol0/application/command/MidiNoteCommand.py
--rw-r--r--   0        0        0      147 2023-06-04 10:45:57.583845 protocol0-1.0.13/protocol0/application/command/PlayPauseSongCommand.py
--rw-r--r--   0        0        0      149 2023-06-04 10:45:57.584884 protocol0-1.0.13/protocol0/application/command/RecordUnlimitedCommand.py
--rw-r--r--   0        0        0      146 2023-06-04 10:45:57.586900 protocol0-1.0.13/protocol0/application/command/ReloadScriptCommand.py
--rw-r--r--   0        0        0      147 2023-06-04 10:45:57.587909 protocol0-1.0.13/protocol0/application/command/ResetPlaybackCommand.py
--rw-r--r--   0        0        0      527 2023-06-04 10:45:57.588910 protocol0-1.0.13/protocol0/application/command/ScrollScenePositionCommand.py
--rw-r--r--   0        0        0      293 2023-06-04 10:45:57.590035 protocol0-1.0.13/protocol0/application/command/ScrollScenesCommand.py
--rw-r--r--   0        0        0      303 2023-06-04 10:45:57.590035 protocol0-1.0.13/protocol0/application/command/ScrollSceneTracksCommand.py
--rw-r--r--   0        0        0      303 2023-06-04 10:45:57.592072 protocol0-1.0.13/protocol0/application/command/ScrollTrackVolumeCommand.py
--rw-r--r--   0        0        0      310 2023-06-04 10:45:57.593196 protocol0-1.0.13/protocol0/application/command/SelectOrLoadDeviceCommand.py
--rw-r--r--   0        0        0      291 2023-06-04 10:45:57.594251 protocol0-1.0.13/protocol0/application/command/SelectTrackCommand.py
--rw-r--r--   0        0        0     1641 2023-06-04 10:45:57.595240 protocol0-1.0.13/protocol0/application/command/SerializableCommand.py
--rw-r--r--   0        0        0      297 2023-06-04 10:45:57.596985 protocol0-1.0.13/protocol0/application/command/ShowAutomationCommand.py
--rw-r--r--   0        0        0      148 2023-06-04 10:45:57.597931 protocol0-1.0.13/protocol0/application/command/ShowInstrumentCommand.py
--rw-r--r--   0        0        0      284 2023-06-04 10:45:57.598925 protocol0-1.0.13/protocol0/application/command/ShowMessageCommand.py
--rw-r--r--   0        0        0      143 2023-06-04 10:45:57.599929 protocol0-1.0.13/protocol0/application/command/ToggleArmCommand.py
--rw-r--r--   0        0        0      145 2023-06-04 10:45:57.600679 protocol0-1.0.13/protocol0/application/command/ToggleNotesCommand.py
--rw-r--r--   0        0        0      154 2023-06-04 10:45:57.601689 protocol0-1.0.13/protocol0/application/command/ToggleReferenceTrackCommand.py
--rw-r--r--   0        0        0      149 2023-06-04 10:45:57.603768 protocol0-1.0.13/protocol0/application/command/ToggleSceneLoopCommand.py
--rw-r--r--   0        0        0      153 2023-06-04 10:45:57.604688 protocol0-1.0.13/protocol0/application/command/UnfoldSelectedSceneCommand.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.646726 protocol0-1.0.13/protocol0/application/command_handler/__init__.py
--rw-r--r--   0        0        0      539 2023-06-04 10:45:57.606688 protocol0-1.0.13/protocol0/application/command_handler/BounceTrackToAudioCommandHandler.py
--rw-r--r--   0        0        0      826 2023-06-04 10:45:57.607740 protocol0-1.0.13/protocol0/application/command_handler/CheckAudioExportValidCommandHandler.py
--rw-r--r--   0        0        0      443 2023-06-04 10:45:57.610241 protocol0-1.0.13/protocol0/application/command_handler/CommandHandlerInterface.py
--rw-r--r--   0        0        0      542 2023-06-04 10:45:57.612239 protocol0-1.0.13/protocol0/application/command_handler/DrumRackToSimplerCommandHandler.py
--rw-r--r--   0        0        0      568 2023-06-04 10:45:57.612626 protocol0-1.0.13/protocol0/application/command_handler/EmitBackendEventCommandHandler.py
--rw-r--r--   0        0        0     1918 2023-06-04 10:45:57.613873 protocol0-1.0.13/protocol0/application/command_handler/FireSceneToPositionCommandHandler.py
--rw-r--r--   0        0        0      546 2023-06-04 10:45:57.615884 protocol0-1.0.13/protocol0/application/command_handler/FireSelectedSceneCommandHandler.py
--rw-r--r--   0        0        0      435 2023-06-04 10:45:57.616870 protocol0-1.0.13/protocol0/application/command_handler/GetSetStateCommandHandler.py
--rw-r--r--   0        0        0      456 2023-06-04 10:45:57.618217 protocol0-1.0.13/protocol0/application/command_handler/GoToGroupTrackCommandHandler.py
--rw-r--r--   0        0        0      529 2023-06-04 10:45:57.619187 protocol0-1.0.13/protocol0/application/command_handler/LoadDeviceCommandHandler.py
--rw-r--r--   0        0        0      714 2023-06-04 10:45:57.620185 protocol0-1.0.13/protocol0/application/command_handler/LoadDrumRackCommandHandler.py
--rw-r--r--   0        0        0      543 2023-06-04 10:45:57.621185 protocol0-1.0.13/protocol0/application/command_handler/LoadMatchingTrackCommandHandler.py
--rw-r--r--   0        0        0      557 2023-06-04 10:45:57.622862 protocol0-1.0.13/protocol0/application/command_handler/LoadMinitaurCommandHandler.py
--rw-r--r--   0        0        0      529 2023-06-04 10:45:57.622862 protocol0-1.0.13/protocol0/application/command_handler/LoadRev2CommandHandler.py
--rw-r--r--   0        0        0     1641 2023-06-04 10:45:57.624221 protocol0-1.0.13/protocol0/application/command_handler/MidiNoteCommandHandler.py
--rw-r--r--   0        0        0      483 2023-06-04 10:45:57.625823 protocol0-1.0.13/protocol0/application/command_handler/PlayPauseSongCommandHandler.py
--rw-r--r--   0        0        0      670 2023-06-04 10:45:57.627331 protocol0-1.0.13/protocol0/application/command_handler/RecordUnlimitedCommandHandler.py
--rw-r--r--   0        0        0      796 2023-06-04 10:45:57.628329 protocol0-1.0.13/protocol0/application/command_handler/ReloadScriptCommandHandler.py
--rw-r--r--   0        0        0      465 2023-06-04 10:45:57.628778 protocol0-1.0.13/protocol0/application/command_handler/ResetPlaybackCommandHandler.py
--rw-r--r--   0        0        0      590 2023-06-04 10:45:57.630529 protocol0-1.0.13/protocol0/application/command_handler/ScrollScenePositionCommandHandler.py
--rw-r--r--   0        0        0      481 2023-06-04 10:45:57.632529 protocol0-1.0.13/protocol0/application/command_handler/ScrollScenesCommandHandler.py
--rw-r--r--   0        0        0      447 2023-06-04 10:45:57.631529 protocol0-1.0.13/protocol0/application/command_handler/ScrollSceneTracksCommandHandler.py
--rw-r--r--   0        0        0      457 2023-06-04 10:45:57.633529 protocol0-1.0.13/protocol0/application/command_handler/ScrollTrackVolumeCommandHandler.py
--rw-r--r--   0        0        0      614 2023-06-04 10:45:57.635122 protocol0-1.0.13/protocol0/application/command_handler/SelectOrLoadDeviceCommandHandler.py
--rw-r--r--   0        0        0      611 2023-06-04 10:45:57.636852 protocol0-1.0.13/protocol0/application/command_handler/SelectTrackCommandHandler.py
--rw-r--r--   0        0        0      505 2023-06-04 10:45:57.637892 protocol0-1.0.13/protocol0/application/command_handler/ShowAutomationCommandHandler.py
--rw-r--r--   0        0        0      555 2023-06-04 10:45:57.638900 protocol0-1.0.13/protocol0/application/command_handler/ShowInstrumentCommandHandler.py
--rw-r--r--   0        0        0      428 2023-06-04 10:45:57.640471 protocol0-1.0.13/protocol0/application/command_handler/ShowMessageCommandHandler.py
--rw-r--r--   0        0        0      505 2023-06-04 10:45:57.641521 protocol0-1.0.13/protocol0/application/command_handler/ToggleArmCommandJHandler.py
--rw-r--r--   0        0        0      400 2023-06-04 10:45:57.642495 protocol0-1.0.13/protocol0/application/command_handler/ToggleNotesCommandHandler.py
--rw-r--r--   0        0        0      432 2023-06-04 10:45:57.643503 protocol0-1.0.13/protocol0/application/command_handler/ToggleReferenceTrackCommandHandler.py
--rw-r--r--   0        0        0      487 2023-06-04 10:45:57.644480 protocol0-1.0.13/protocol0/application/command_handler/ToggleSceneLoopCommandHandler.py
--rw-r--r--   0        0        0      427 2023-06-04 10:45:57.646726 protocol0-1.0.13/protocol0/application/command_handler/UnfoldSelectedSceneCommandHandler.py
--rw-r--r--   0        0        0     4453 2023-06-04 10:45:57.557129 protocol0-1.0.13/protocol0/application/CommandBus.py
--rw-r--r--   0        0        0     1420 2023-06-04 10:45:57.558132 protocol0-1.0.13/protocol0/application/CommandBusHistory.py
--rw-r--r--   0        0        0    12580 2023-06-04 10:45:57.560430 protocol0-1.0.13/protocol0/application/Container.py
--rw-r--r--   0        0        0      196 2023-06-04 10:45:57.561438 protocol0-1.0.13/protocol0/application/ContainerInterface.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.655439 protocol0-1.0.13/protocol0/application/control_surface/__init__.py
--rw-r--r--   0        0        0      772 2023-06-04 10:45:57.648426 protocol0-1.0.13/protocol0/application/control_surface/ActionGroupFactory.py
--rw-r--r--   0        0        0     2750 2023-06-04 10:45:57.650263 protocol0-1.0.13/protocol0/application/control_surface/ActionGroupInterface.py
--rw-r--r--   0        0        0     2983 2023-06-04 10:45:57.652338 protocol0-1.0.13/protocol0/application/control_surface/EncoderAction.py
--rw-r--r--   0        0        0      173 2023-06-04 10:45:57.653434 protocol0-1.0.13/protocol0/application/control_surface/EncoderMoveEnum.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.665941 protocol0-1.0.13/protocol0/application/control_surface/group/__init__.py
--rw-r--r--   0        0        0     1356 2023-06-04 10:45:57.656442 protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupClip.py
--rw-r--r--   0        0        0     1268 2023-06-04 10:45:57.657549 protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupCut.py
--rw-r--r--   0        0        0      892 2023-06-04 10:45:57.658700 protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupFix.py
--rw-r--r--   0        0        0     1240 2023-06-04 10:45:57.660938 protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupLog.py
--rw-r--r--   0        0        0     3931 2023-06-04 10:45:57.661994 protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupMain.py
--rw-r--r--   0        0        0      595 2023-06-04 10:45:57.662946 protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupSample.py
--rw-r--r--   0        0        0      985 2023-06-04 10:45:57.663984 protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupSet.py
--rw-r--r--   0        0        0     2120 2023-06-04 10:45:57.664986 protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupTest.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.667947 protocol0-1.0.13/protocol0/application/control_surface/group/legacy/__init__.py
--rw-r--r--   0        0        0     1090 2023-06-04 10:45:57.666989 protocol0-1.0.13/protocol0/application/control_surface/group/legacy/ActionGroupPreset.py
--rw-r--r--   0        0        0     5488 2023-06-04 10:45:57.654464 protocol0-1.0.13/protocol0/application/control_surface/MultiEncoder.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.671223 protocol0-1.0.13/protocol0/application/error/__init__.py
--rw-r--r--   0        0        0     6156 2023-06-04 10:45:57.670232 protocol0-1.0.13/protocol0/application/error/ErrorService.py
--rw-r--r--   0        0        0      370 2023-06-04 10:45:57.672260 protocol0-1.0.13/protocol0/application/main.py
--rw-r--r--   0        0        0     1968 2023-06-04 10:45:57.562439 protocol0-1.0.13/protocol0/application/Protocol0.py
--rw-r--r--   0        0        0     1940 2023-06-04 10:45:57.563759 protocol0-1.0.13/protocol0/application/Protocol0Midi.py
--rw-r--r--   0        0        0       64 2023-06-04 10:45:57.679519 protocol0-1.0.13/protocol0/application/push2/__init__.py
--rw-r--r--   0        0        0     5916 2023-06-04 10:45:57.673855 protocol0-1.0.13/protocol0/application/push2/P0Push2.py
--rw-r--r--   0        0        0     4078 2023-06-04 10:45:57.675155 protocol0-1.0.13/protocol0/application/push2/P0SessionRingTrackProvider.py
--rw-r--r--   0        0        0      678 2023-06-04 10:45:57.676182 protocol0-1.0.13/protocol0/application/push2/P0ShowInstrumentMode.py
--rw-r--r--   0        0        0      575 2023-06-04 10:45:57.677560 protocol0-1.0.13/protocol0/application/push2/P0TrackListComponent.py
--rw-r--r--   0        0        0      476 2023-06-04 10:45:57.678518 protocol0-1.0.13/protocol0/application/push2/P0TransportComponent.py
--rw-r--r--   0        0        0       50 2023-06-04 10:45:57.564805 protocol0-1.0.13/protocol0/application/ScriptDisconnectedEvent.py
--rw-r--r--   0        0        0       52 2023-06-04 10:45:57.565833 protocol0-1.0.13/protocol0/application/ScriptResetActivatedEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.680523 protocol0-1.0.13/protocol0/domain/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.690394 protocol0-1.0.13/protocol0/domain/audit/__init__.py
--rw-r--r--   0        0        0     4967 2023-06-04 10:45:57.682154 protocol0-1.0.13/protocol0/domain/audit/AudioLatencyAnalyzerService.py
--rw-r--r--   0        0        0     8617 2023-06-04 10:45:57.686202 protocol0-1.0.13/protocol0/domain/audit/LogService.py
--rw-r--r--   0        0        0     1317 2023-06-04 10:45:57.684149 protocol0-1.0.13/protocol0/domain/audit/LOMAnalyzerService.py
--rw-r--r--   0        0        0     2383 2023-06-04 10:45:57.687207 protocol0-1.0.13/protocol0/domain/audit/SetFixerService.py
--rw-r--r--   0        0        0     3309 2023-06-04 10:45:57.689152 protocol0-1.0.13/protocol0/domain/audit/SetUpgradeService.py
--rw-r--r--   0        0        0      412 2023-06-04 10:45:57.690321 protocol0-1.0.13/protocol0/domain/audit/SongStatsService.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.701613 protocol0-1.0.13/protocol0/domain/audit/stats/__init__.py
--rw-r--r--   0        0        0     1429 2023-06-04 10:45:57.691947 protocol0-1.0.13/protocol0/domain/audit/stats/ClipStats.py
--rw-r--r--   0        0        0     3356 2023-06-04 10:45:57.692974 protocol0-1.0.13/protocol0/domain/audit/stats/DeviceStats.py
--rw-r--r--   0        0        0     2275 2023-06-04 10:45:57.695016 protocol0-1.0.13/protocol0/domain/audit/stats/SampleStats.py
--rw-r--r--   0        0        0     1014 2023-06-04 10:45:57.696600 protocol0-1.0.13/protocol0/domain/audit/stats/SceneStats.py
--rw-r--r--   0        0        0      995 2023-06-04 10:45:57.698627 protocol0-1.0.13/protocol0/domain/audit/stats/SongStats.py
--rw-r--r--   0        0        0      180 2023-06-04 10:45:57.699612 protocol0-1.0.13/protocol0/domain/audit/stats/Stats.py
--rw-r--r--   0        0        0      900 2023-06-04 10:45:57.700613 protocol0-1.0.13/protocol0/domain/audit/stats/TrackStats.py
--rw-r--r--   0        0        0      337 2023-06-04 10:45:57.702662 protocol0-1.0.13/protocol0/domain/audit/utils.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.703673 protocol0-1.0.13/protocol0/domain/lom/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.721607 protocol0-1.0.13/protocol0/domain/lom/clip/__init__.py
--rw-r--r--   0        0        0     2441 2023-06-04 10:45:57.705981 protocol0-1.0.13/protocol0/domain/lom/clip/AudioClip.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.725393 protocol0-1.0.13/protocol0/domain/lom/clip/automation/__init__.py
--rw-r--r--   0        0        0     3719 2023-06-04 10:45:57.723658 protocol0-1.0.13/protocol0/domain/lom/clip/automation/ClipAutomation.py
--rw-r--r--   0        0        0     1888 2023-06-04 10:45:57.724335 protocol0-1.0.13/protocol0/domain/lom/clip/automation/ClipAutomationEnvelope.py
--rw-r--r--   0        0        0     7866 2023-06-04 10:45:57.707359 protocol0-1.0.13/protocol0/domain/lom/clip/Clip.py
--rw-r--r--   0        0        0      913 2023-06-04 10:45:57.708370 protocol0-1.0.13/protocol0/domain/lom/clip/ClipAppearance.py
--rw-r--r--   0        0        0      160 2023-06-04 10:45:57.709373 protocol0-1.0.13/protocol0/domain/lom/clip/ClipColorEnum.py
--rw-r--r--   0        0        0      183 2023-06-04 10:45:57.710394 protocol0-1.0.13/protocol0/domain/lom/clip/ClipConfig.py
--rw-r--r--   0        0        0      287 2023-06-04 10:45:57.711366 protocol0-1.0.13/protocol0/domain/lom/clip/ClipCreatedOrDeletedEvent.py
--rw-r--r--   0        0        0       50 2023-06-04 10:45:57.713367 protocol0-1.0.13/protocol0/domain/lom/clip/ClipEnvelopeShowedEvent.py
--rw-r--r--   0        0        0     4219 2023-06-04 10:45:57.714438 protocol0-1.0.13/protocol0/domain/lom/clip/ClipInfo.py
--rw-r--r--   0        0        0     5558 2023-06-04 10:45:57.714893 protocol0-1.0.13/protocol0/domain/lom/clip/ClipLoop.py
--rw-r--r--   0        0        0     4087 2023-06-04 10:45:57.716003 protocol0-1.0.13/protocol0/domain/lom/clip/ClipName.py
--rw-r--r--   0        0        0      920 2023-06-04 10:45:57.717060 protocol0-1.0.13/protocol0/domain/lom/clip/ClipPlayingPosition.py
--rw-r--r--   0        0        0      192 2023-06-04 10:45:57.718013 protocol0-1.0.13/protocol0/domain/lom/clip/ClipSlotSelectedEvent.py
--rw-r--r--   0        0        0     2110 2023-06-04 10:45:57.720009 protocol0-1.0.13/protocol0/domain/lom/clip/ClipTail.py
--rw-r--r--   0        0        0     7368 2023-06-04 10:45:57.721102 protocol0-1.0.13/protocol0/domain/lom/clip/MidiClip.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.736330 protocol0-1.0.13/protocol0/domain/lom/clip_slot/__init__.py
--rw-r--r--   0        0        0     2644 2023-06-04 10:45:57.728387 protocol0-1.0.13/protocol0/domain/lom/clip_slot/AudioClipSlot.py
--rw-r--r--   0        0        0     5709 2023-06-04 10:45:57.729346 protocol0-1.0.13/protocol0/domain/lom/clip_slot/ClipSlot.py
--rw-r--r--   0        0        0      736 2023-06-04 10:45:57.730448 protocol0-1.0.13/protocol0/domain/lom/clip_slot/ClipSlotAppearance.py
--rw-r--r--   0        0        0      171 2023-06-04 10:45:57.733317 protocol0-1.0.13/protocol0/domain/lom/clip_slot/ClipSlotHasClipEvent.py
--rw-r--r--   0        0        0      401 2023-06-04 10:45:57.734375 protocol0-1.0.13/protocol0/domain/lom/clip_slot/MidiClipSlot.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.763299 protocol0-1.0.13/protocol0/domain/lom/device/__init__.py
--rw-r--r--   0        0        0     4725 2023-06-04 10:45:57.737316 protocol0-1.0.13/protocol0/domain/lom/device/Device.py
--rw-r--r--   0        0        0     1445 2023-06-04 10:45:57.739369 protocol0-1.0.13/protocol0/domain/lom/device/DeviceChain.py
--rw-r--r--   0        0        0     6848 2023-06-04 10:45:57.740369 protocol0-1.0.13/protocol0/domain/lom/device/DeviceDisplayService.py
--rw-r--r--   0        0        0    12713 2023-06-04 10:45:57.742747 protocol0-1.0.13/protocol0/domain/lom/device/DeviceEnum.py
--rw-r--r--   0        0        0      585 2023-06-04 10:45:57.743754 protocol0-1.0.13/protocol0/domain/lom/device/DeviceEnumGroup.py
--rw-r--r--   0        0        0      217 2023-06-04 10:45:57.744759 protocol0-1.0.13/protocol0/domain/lom/device/DeviceLoadedEvent.py
--rw-r--r--   0        0        0     4628 2023-06-04 10:45:57.745872 protocol0-1.0.13/protocol0/domain/lom/device/DeviceService.py
--rw-r--r--   0        0        0     2166 2023-06-04 10:45:57.747930 protocol0-1.0.13/protocol0/domain/lom/device/DrumPad.py
--rw-r--r--   0        0        0     1193 2023-06-04 10:45:57.748925 protocol0-1.0.13/protocol0/domain/lom/device/DrumRackDevice.py
--rw-r--r--   0        0        0       46 2023-06-04 10:45:57.749925 protocol0-1.0.13/protocol0/domain/lom/device/DrumRackLoadedEvent.py
--rw-r--r--   0        0        0     1601 2023-06-04 10:45:57.751879 protocol0-1.0.13/protocol0/domain/lom/device/DrumRackSampleService.py
--rw-r--r--   0        0        0     7314 2023-06-04 10:45:57.753380 protocol0-1.0.13/protocol0/domain/lom/device/DrumRackService.py
--rw-r--r--   0        0        0     1393 2023-06-04 10:45:57.754713 protocol0-1.0.13/protocol0/domain/lom/device/MixerDevice.py
--rw-r--r--   0        0        0     1290 2023-06-04 10:45:57.755801 protocol0-1.0.13/protocol0/domain/lom/device/PluginDevice.py
--rw-r--r--   0        0        0     1822 2023-06-04 10:45:57.756778 protocol0-1.0.13/protocol0/domain/lom/device/RackDevice.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.760401 protocol0-1.0.13/protocol0/domain/lom/device/Sample/__init__.py
--rw-r--r--   0        0        0     1419 2023-06-04 10:45:57.758833 protocol0-1.0.13/protocol0/domain/lom/device/Sample/Sample.py
--rw-r--r--   0        0        0      346 2023-06-04 10:45:57.759368 protocol0-1.0.13/protocol0/domain/lom/device/Sample/SampleNotFoundError.py
--rw-r--r--   0        0        0     1812 2023-06-04 10:45:57.763299 protocol0-1.0.13/protocol0/domain/lom/device/SimplerDevice.py
--rw-r--r--   0        0        0     5436 2023-06-04 10:45:57.761219 protocol0-1.0.13/protocol0/domain/lom/device/SimpleTrackDevices.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.771500 protocol0-1.0.13/protocol0/domain/lom/device_parameter/__init__.py
--rw-r--r--   0        0        0     4609 2023-06-04 10:45:57.766344 protocol0-1.0.13/protocol0/domain/lom/device_parameter/DeviceParameter.py
--rw-r--r--   0        0        0     4124 2023-06-04 10:45:57.767305 protocol0-1.0.13/protocol0/domain/lom/device_parameter/DeviceParameterEnum.py
--rw-r--r--   0        0        0      925 2023-06-04 10:45:57.770075 protocol0-1.0.13/protocol0/domain/lom/device_parameter/DeviceParameterValue.py
--rw-r--r--   0        0        0     1431 2023-06-04 10:45:57.771500 protocol0-1.0.13/protocol0/domain/lom/device_parameter/LinkedDeviceParameters.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.780156 protocol0-1.0.13/protocol0/domain/lom/instrument/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.794364 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/__init__.py
--rw-r--r--   0        0        0      604 2023-06-04 10:45:57.782374 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentAddictiveKeys.py
--rw-r--r--   0        0        0      500 2023-06-04 10:45:57.784360 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentDrumRack.py
--rw-r--r--   0        0        0      394 2023-06-04 10:45:57.786341 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentKontakt.py
--rw-r--r--   0        0        0      737 2023-06-04 10:45:57.787353 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentMinitaur.py
--rw-r--r--   0        0        0      382 2023-06-04 10:45:57.788367 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentOpus.py
--rw-r--r--   0        0        0      382 2023-06-04 10:45:57.789389 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentPlay.py
--rw-r--r--   0        0        0     2994 2023-06-04 10:45:57.790390 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentRev2.py
--rw-r--r--   0        0        0      290 2023-06-04 10:45:57.791347 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentSampler.py
--rw-r--r--   0        0        0      505 2023-06-04 10:45:57.792383 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentSerum.py
--rw-r--r--   0        0        0     1013 2023-06-04 10:45:57.793339 protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentSimpler.py
--rw-r--r--   0        0        0      252 2023-06-04 10:45:57.773816 protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentActivatedEvent.py
--rw-r--r--   0        0        0      235 2023-06-04 10:45:57.774819 protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentColorEnum.py
--rw-r--r--   0        0        0     4475 2023-06-04 10:45:57.776803 protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentDisplayService.py
--rw-r--r--   0        0        0     4273 2023-06-04 10:45:57.778152 protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentFactory.py
--rw-r--r--   0        0        0     4480 2023-06-04 10:45:57.779152 protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentInterface.py
--rw-r--r--   0        0        0       50 2023-06-04 10:45:57.780156 protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentSelectedEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.803314 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/__init__.py
--rw-r--r--   0        0        0      956 2023-06-04 10:45:57.795457 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/InstrumentPreset.py
--rw-r--r--   0        0        0     3209 2023-06-04 10:45:57.797324 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/InstrumentPresetList.py
--rw-r--r--   0        0        0     1957 2023-06-04 10:45:57.799353 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/InstrumentPresetScrollerService.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.811182 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_changer/__init__.py
--rw-r--r--   0        0        0      812 2023-06-04 10:45:57.804773 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py
--rw-r--r--   0        0        0      498 2023-06-04 10:45:57.806804 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_changer/PresetChangerInterface.py
--rw-r--r--   0        0        0      811 2023-06-04 10:45:57.809166 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py
--rw-r--r--   0        0        0      581 2023-06-04 10:45:57.810171 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.820462 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/__init__.py
--rw-r--r--   0        0        0     1982 2023-06-04 10:45:57.812607 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py
--rw-r--r--   0        0        0      613 2023-06-04 10:45:57.813619 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/FilePresetImporter.py
--rw-r--r--   0        0        0      387 2023-06-04 10:45:57.815883 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/NullPresetImporter.py
--rw-r--r--   0        0        0      699 2023-06-04 10:45:57.816260 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py
--rw-r--r--   0        0        0     1854 2023-06-04 10:45:57.819453 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py
--rw-r--r--   0        0        0      812 2023-06-04 10:45:57.818271 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/PresetImportInterface.py
--rw-r--r--   0        0        0      686 2023-06-04 10:45:57.820462 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.825961 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_initializer/__init__.py
--rw-r--r--   0        0        0      627 2023-06-04 10:45:57.822498 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py
--rw-r--r--   0        0        0      575 2023-06-04 10:45:57.823914 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py
--rw-r--r--   0        0        0      611 2023-06-04 10:45:57.824959 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py
--rw-r--r--   0        0        0      171 2023-06-04 10:45:57.800351 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/PresetDisplayOptionEnum.py
--rw-r--r--   0        0        0      155 2023-06-04 10:45:57.801397 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/PresetProgramSelectedEvent.py
--rw-r--r--   0        0        0      145 2023-06-04 10:45:57.803314 protocol0-1.0.13/protocol0/domain/lom/instrument/preset/SampleSelectedEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.827732 protocol0-1.0.13/protocol0/domain/lom/loop/__init__.py
--rw-r--r--   0        0        0      915 2023-06-04 10:45:57.827732 protocol0-1.0.13/protocol0/domain/lom/loop/LoopableInterface.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.830739 protocol0-1.0.13/protocol0/domain/lom/note/__init__.py
--rw-r--r--   0        0        0     3578 2023-06-04 10:45:57.829785 protocol0-1.0.13/protocol0/domain/lom/note/Note.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.833907 protocol0-1.0.13/protocol0/domain/lom/sample/__init__.py
--rw-r--r--   0        0        0     3492 2023-06-04 10:45:57.831770 protocol0-1.0.13/protocol0/domain/lom/sample/SampleCategory.py
--rw-r--r--   0        0        0     1235 2023-06-04 10:45:57.832742 protocol0-1.0.13/protocol0/domain/lom/sample/SampleCategoryEnum.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.859520 protocol0-1.0.13/protocol0/domain/lom/scene/__init__.py
--rw-r--r--   0        0        0     1199 2023-06-04 10:45:57.834937 protocol0-1.0.13/protocol0/domain/lom/scene/LoopingSceneToggler.py
--rw-r--r--   0        0        0      372 2023-06-04 10:45:57.836705 protocol0-1.0.13/protocol0/domain/lom/scene/NextSceneStartedEvent.py
--rw-r--r--   0        0        0       51 2023-06-04 10:45:57.838723 protocol0-1.0.13/protocol0/domain/lom/scene/PlayingSceneChangedEvent.py
--rw-r--r--   0        0        0     2903 2023-06-04 10:45:57.839751 protocol0-1.0.13/protocol0/domain/lom/scene/PlayingSceneFacade.py
--rw-r--r--   0        0        0     8521 2023-06-04 10:45:57.840750 protocol0-1.0.13/protocol0/domain/lom/scene/Scene.py
--rw-r--r--   0        0        0      887 2023-06-04 10:45:57.841452 protocol0-1.0.13/protocol0/domain/lom/scene/SceneAppearance.py
--rw-r--r--   0        0        0     3472 2023-06-04 10:45:57.843216 protocol0-1.0.13/protocol0/domain/lom/scene/SceneClips.py
--rw-r--r--   0        0        0      735 2023-06-04 10:45:57.844263 protocol0-1.0.13/protocol0/domain/lom/scene/SceneCropScroller.py
--rw-r--r--   0        0        0      202 2023-06-04 10:45:57.845264 protocol0-1.0.13/protocol0/domain/lom/scene/SceneFiredEvent.py
--rw-r--r--   0        0        0      263 2023-06-04 10:45:57.846254 protocol0-1.0.13/protocol0/domain/lom/scene/SceneLastBarPassedEvent.py
--rw-r--r--   0        0        0     2376 2023-06-04 10:45:57.847262 protocol0-1.0.13/protocol0/domain/lom/scene/SceneLength.py
--rw-r--r--   0        0        0     3560 2023-06-04 10:45:57.848324 protocol0-1.0.13/protocol0/domain/lom/scene/SceneName.py
--rw-r--r--   0        0        0     5743 2023-06-04 10:45:57.849839 protocol0-1.0.13/protocol0/domain/lom/scene/ScenePlaybackService.py
--rw-r--r--   0        0        0     1997 2023-06-04 10:45:57.850880 protocol0-1.0.13/protocol0/domain/lom/scene/ScenePlayingState.py
--rw-r--r--   0        0        0       53 2023-06-04 10:45:57.851893 protocol0-1.0.13/protocol0/domain/lom/scene/ScenePositionScrolledEvent.py
--rw-r--r--   0        0        0     1767 2023-06-04 10:45:57.853467 protocol0-1.0.13/protocol0/domain/lom/scene/ScenePositionScroller.py
--rw-r--r--   0        0        0     6160 2023-06-04 10:45:57.854514 protocol0-1.0.13/protocol0/domain/lom/scene/SceneService.py
--rw-r--r--   0        0        0       44 2023-06-04 10:45:57.858472 protocol0-1.0.13/protocol0/domain/lom/scene/ScenesMappedEvent.py
--rw-r--r--   0        0        0     3355 2023-06-04 10:45:57.855477 protocol0-1.0.13/protocol0/domain/lom/scene/SceneWindow.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.866109 protocol0-1.0.13/protocol0/domain/lom/set/__init__.py
--rw-r--r--   0        0        0     4599 2023-06-04 10:45:57.860605 protocol0-1.0.13/protocol0/domain/lom/set/AbletonSet.py
--rw-r--r--   0        0        0      270 2023-06-04 10:45:57.861519 protocol0-1.0.13/protocol0/domain/lom/set/AbletonSetChangedEvent.py
--rw-r--r--   0        0        0      420 2023-06-04 10:45:57.863528 protocol0-1.0.13/protocol0/domain/lom/set/MixingService.py
--rw-r--r--   0        0        0     6197 2023-06-04 10:45:57.866109 protocol0-1.0.13/protocol0/domain/lom/set/SessionToArrangementService.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.872912 protocol0-1.0.13/protocol0/domain/lom/song/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.887048 protocol0-1.0.13/protocol0/domain/lom/song/components/__init__.py
--rw-r--r--   0        0        0     2528 2023-06-04 10:45:57.874402 protocol0-1.0.13/protocol0/domain/lom/song/components/ClipComponent.py
--rw-r--r--   0        0        0     2480 2023-06-04 10:45:57.875793 protocol0-1.0.13/protocol0/domain/lom/song/components/DeviceComponent.py
--rw-r--r--   0        0        0     5230 2023-06-04 10:45:57.877999 protocol0-1.0.13/protocol0/domain/lom/song/components/PlaybackComponent.py
--rw-r--r--   0        0        0     1177 2023-06-04 10:45:57.879009 protocol0-1.0.13/protocol0/domain/lom/song/components/QuantizationComponent.py
--rw-r--r--   0        0        0     2950 2023-06-04 10:45:57.880010 protocol0-1.0.13/protocol0/domain/lom/song/components/RecordingComponent.py
--rw-r--r--   0        0        0     2288 2023-06-04 10:45:57.881044 protocol0-1.0.13/protocol0/domain/lom/song/components/SceneComponent.py
--rw-r--r--   0        0        0     2543 2023-06-04 10:45:57.882006 protocol0-1.0.13/protocol0/domain/lom/song/components/SceneCrudComponent.py
--rw-r--r--   0        0        0     1179 2023-06-04 10:45:57.883047 protocol0-1.0.13/protocol0/domain/lom/song/components/TempoComponent.py
--rw-r--r--   0        0        0     4790 2023-06-04 10:45:57.884024 protocol0-1.0.13/protocol0/domain/lom/song/components/TrackComponent.py
--rw-r--r--   0        0        0     2028 2023-06-04 10:45:57.886036 protocol0-1.0.13/protocol0/domain/lom/song/components/TrackCrudComponent.py
--rw-r--r--   0        0        0       47 2023-06-04 10:45:57.868938 protocol0-1.0.13/protocol0/domain/lom/song/SongInitializedEvent.py
--rw-r--r--   0        0        0     2090 2023-06-04 10:45:57.867906 protocol0-1.0.13/protocol0/domain/lom/song/SongInitService.py
--rw-r--r--   0        0        0       43 2023-06-04 10:45:57.869923 protocol0-1.0.13/protocol0/domain/lom/song/SongStartedEvent.py
--rw-r--r--   0        0        0       43 2023-06-04 10:45:57.871952 protocol0-1.0.13/protocol0/domain/lom/song/SongStoppedEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.899961 protocol0-1.0.13/protocol0/domain/lom/track/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.906980 protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/__init__.py
--rw-r--r--   0        0        0     1509 2023-06-04 10:45:57.901978 protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/AbstrackTrackArmState.py
--rw-r--r--   0        0        0     6108 2023-06-04 10:45:57.902939 protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/AbstractTrack.py
--rw-r--r--   0        0        0     2203 2023-06-04 10:45:57.904964 protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/AbstractTrackAppearance.py
--rw-r--r--   0        0        0       56 2023-06-04 10:45:57.905965 protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/AbstractTrackNameUpdatedEvent.py
--rw-r--r--   0        0        0      179 2023-06-04 10:45:57.906980 protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/AbstractTrackSelectedEvent.py
--rw-r--r--   0        0        0      135 2023-06-04 10:45:57.888738 protocol0-1.0.13/protocol0/domain/lom/track/CurrentMonitoringStateEnum.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.915229 protocol0-1.0.13/protocol0/domain/lom/track/group_track/__init__.py
--rw-r--r--   0        0        0     3797 2023-06-04 10:45:57.909040 protocol0-1.0.13/protocol0/domain/lom/track/group_track/AbstractGroupTrack.py
--rw-r--r--   0        0        0      385 2023-06-04 10:45:57.910200 protocol0-1.0.13/protocol0/domain/lom/track/group_track/DrumsTrack.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.929035 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/__init__.py
--rw-r--r--   0        0        0      271 2023-06-04 10:45:57.919261 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtArmedEvent.py
--rw-r--r--   0        0        0     2284 2023-06-04 10:45:57.918245 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtArmState.py
--rw-r--r--   0        0        0     4340 2023-06-04 10:45:57.925796 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExternalSynthTrack.py
--rw-r--r--   0        0        0     2589 2023-06-04 10:45:57.920993 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtMatchingTrack.py
--rw-r--r--   0        0        0     3000 2023-06-04 10:45:57.921994 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py
--rw-r--r--   0        0        0     1952 2023-06-04 10:45:57.922784 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtMonitoringState.py
--rw-r--r--   0        0        0     2115 2023-06-04 10:45:57.923790 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtSoloState.py
--rw-r--r--   0        0        0      662 2023-06-04 10:45:57.926791 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py
--rw-r--r--   0        0        0      847 2023-06-04 10:45:57.928015 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py
--rw-r--r--   0        0        0      759 2023-06-04 10:45:57.929035 protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.940091 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/__init__.py
--rw-r--r--   0        0        0     2002 2023-06-04 10:45:57.931555 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py
--rw-r--r--   0        0        0     3644 2023-06-04 10:45:57.932599 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py
--rw-r--r--   0        0        0      645 2023-06-04 10:45:57.934573 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py
--rw-r--r--   0        0        0     2055 2023-06-04 10:45:57.935619 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackInterface.py
--rw-r--r--   0        0        0     2310 2023-06-04 10:45:57.936585 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackRouter.py
--rw-r--r--   0        0        0     7279 2023-06-04 10:45:57.938582 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackService.py
--rw-r--r--   0        0        0      956 2023-06-04 10:45:57.939645 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py
--rw-r--r--   0        0        0     2159 2023-06-04 10:45:57.941095 protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/utils.py
--rw-r--r--   0        0        0      978 2023-06-04 10:45:57.911714 protocol0-1.0.13/protocol0/domain/lom/track/group_track/NormalGroupMatchingTrack.py
--rw-r--r--   0        0        0     1572 2023-06-04 10:45:57.913055 protocol0-1.0.13/protocol0/domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py
--rw-r--r--   0        0        0     3733 2023-06-04 10:45:57.914210 protocol0-1.0.13/protocol0/domain/lom/track/group_track/NormalGroupTrack.py
--rw-r--r--   0        0        0      155 2023-06-04 10:45:57.915229 protocol0-1.0.13/protocol0/domain/lom/track/group_track/VocalsTrack.py
--rw-r--r--   0        0        0      205 2023-06-04 10:45:57.889495 protocol0-1.0.13/protocol0/domain/lom/track/P0TrackInterface.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.952086 protocol0-1.0.13/protocol0/domain/lom/track/routing/__init__.py
--rw-r--r--   0        0        0      237 2023-06-04 10:45:57.943098 protocol0-1.0.13/protocol0/domain/lom/track/routing/InputRoutingChannelEnum.py
--rw-r--r--   0        0        0      251 2023-06-04 10:45:57.944404 protocol0-1.0.13/protocol0/domain/lom/track/routing/InputRoutingTypeEnum.py
--rw-r--r--   0        0        0      251 2023-06-04 10:45:57.946061 protocol0-1.0.13/protocol0/domain/lom/track/routing/OutputRoutingTypeEnum.py
--rw-r--r--   0        0        0     1786 2023-06-04 10:45:57.947103 protocol0-1.0.13/protocol0/domain/lom/track/routing/RoutingDisplayNameDescriptor.py
--rw-r--r--   0        0        0     3576 2023-06-04 10:45:57.948137 protocol0-1.0.13/protocol0/domain/lom/track/routing/RoutingTrackDescriptor.py
--rw-r--r--   0        0        0      779 2023-06-04 10:45:57.949064 protocol0-1.0.13/protocol0/domain/lom/track/routing/TrackInputRouting.py
--rw-r--r--   0        0        0      595 2023-06-04 10:45:57.950090 protocol0-1.0.13/protocol0/domain/lom/track/routing/TrackOutputRouting.py
--rw-r--r--   0        0        0      441 2023-06-04 10:45:57.951090 protocol0-1.0.13/protocol0/domain/lom/track/routing/TrackRoutingInterface.py
--rw-r--r--   0        0        0       52 2023-06-04 10:45:57.891724 protocol0-1.0.13/protocol0/domain/lom/track/SelectedTrackChangedEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.972856 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.976822 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.978834 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/master/__init__.py
--rw-r--r--   0        0        0     1971 2023-06-04 10:45:57.977834 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/master/MasterTrack.py
--rw-r--r--   0        0        0     4947 2023-06-04 10:45:57.973857 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/SimpleAudioTrack.py
--rw-r--r--   0        0        0      650 2023-06-04 10:45:57.976060 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/SimpleReturnTrack.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.983751 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/special/__init__.py
--rw-r--r--   0        0        0     1253 2023-06-04 10:45:57.982161 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/special/ReferenceTrack.py
--rw-r--r--   0        0        0      397 2023-06-04 10:45:57.983751 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/special/ResamplingTrack.py
--rw-r--r--   0        0        0     2912 2023-06-04 10:45:57.953359 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/AudioToMidiClipMapping.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.986654 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/midi/__init__.py
--rw-r--r--   0        0        0     1566 2023-06-04 10:45:57.985595 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/midi/SimpleMidiTrack.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.988689 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/midi/special/__init__.py
--rw-r--r--   0        0        0     2717 2023-06-04 10:45:57.988689 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/midi/special/UsamoTrack.py
--rw-r--r--   0        0        0     2642 2023-06-04 10:45:57.954693 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleMatchingTrack.py
--rw-r--r--   0        0        0     1568 2023-06-04 10:45:57.956895 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleMatchingTrackCreator.py
--rw-r--r--   0        0        0    16256 2023-06-04 10:45:57.957888 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrack.py
--rw-r--r--   0        0        0      174 2023-06-04 10:45:57.960123 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackArmedEvent.py
--rw-r--r--   0        0        0     1375 2023-06-04 10:45:57.958888 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackArmState.py
--rw-r--r--   0        0        0     1387 2023-06-04 10:45:57.962151 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackClipColorManager.py
--rw-r--r--   0        0        0     1038 2023-06-04 10:45:57.964844 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackClips.py
--rw-r--r--   0        0        0     4738 2023-06-04 10:45:57.963333 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackClipSlots.py
--rw-r--r--   0        0        0      279 2023-06-04 10:45:57.965856 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackCreatedEvent.py
--rw-r--r--   0        0        0      279 2023-06-04 10:45:57.966854 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackDeletedEvent.py
--rw-r--r--   0        0        0      247 2023-06-04 10:45:57.967854 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackFlattenedEvent.py
--rw-r--r--   0        0        0     1219 2023-06-04 10:45:57.968854 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackMonitoringState.py
--rw-r--r--   0        0        0       54 2023-06-04 10:45:57.969856 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackSaveStartedEvent.py
--rw-r--r--   0        0        0      894 2023-06-04 10:45:57.971859 protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackService.py
--rw-r--r--   0        0        0       42 2023-06-04 10:45:57.892742 protocol0-1.0.13/protocol0/domain/lom/track/TrackAddedEvent.py
--rw-r--r--   0        0        0     6094 2023-06-04 10:45:57.893901 protocol0-1.0.13/protocol0/domain/lom/track/TrackAutomationService.py
--rw-r--r--   0        0        0      166 2023-06-04 10:45:57.894600 protocol0-1.0.13/protocol0/domain/lom/track/TrackColorEnum.py
--rw-r--r--   0        0        0      286 2023-06-04 10:45:57.895710 protocol0-1.0.13/protocol0/domain/lom/track/TrackDisconnectedEvent.py
--rw-r--r--   0        0        0     4711 2023-06-04 10:45:57.896723 protocol0-1.0.13/protocol0/domain/lom/track/TrackFactory.py
--rw-r--r--   0        0        0     8779 2023-06-04 10:45:57.897760 protocol0-1.0.13/protocol0/domain/lom/track/TrackMapperService.py
--rw-r--r--   0        0        0     1054 2023-06-04 10:45:57.898935 protocol0-1.0.13/protocol0/domain/lom/track/TrackService.py
--rw-r--r--   0        0        0       44 2023-06-04 10:45:57.899961 protocol0-1.0.13/protocol0/domain/lom/track/TracksMappedEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:57.994476 protocol0-1.0.13/protocol0/domain/lom/validation/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.001537 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/__init__.py
--rw-r--r--   0        0        0      385 2023-06-04 10:45:57.996814 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/AbstractGroupTrackValidator.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.006595 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/external_synth_track/__init__.py
--rw-r--r--   0        0        0     2097 2023-06-04 10:45:58.002971 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py
--rw-r--r--   0        0        0     1735 2023-06-04 10:45:58.004966 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py
--rw-r--r--   0        0        0     2126 2023-06-04 10:45:58.006595 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py
--rw-r--r--   0        0        0      950 2023-06-04 10:45:57.998089 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/SceneValidator.py
--rw-r--r--   0        0        0      938 2023-06-04 10:45:57.999904 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/SimpleAudioTrackValidator.py
--rw-r--r--   0        0        0      413 2023-06-04 10:45:58.000951 protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/SimpleTrackValidator.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.015692 protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/__init__.py
--rw-r--r--   0        0        0     1053 2023-06-04 10:45:58.008387 protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/AggregateValidator.py
--rw-r--r--   0        0        0     1106 2023-06-04 10:45:58.010299 protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/CallbackValidator.py
--rw-r--r--   0        0        0     1570 2023-06-04 10:45:58.012313 protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/DeviceParameterValidator.py
--rw-r--r--   0        0        0     1912 2023-06-04 10:45:58.013680 protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/PropertyValueValidator.py
--rw-r--r--   0        0        0     1355 2023-06-04 10:45:58.014690 protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py
--rw-r--r--   0        0        0     2173 2023-06-04 10:45:57.991020 protocol0-1.0.13/protocol0/domain/lom/validation/ValidatorFactory.py
--rw-r--r--   0        0        0      559 2023-06-04 10:45:57.992298 protocol0-1.0.13/protocol0/domain/lom/validation/ValidatorInterface.py
--rw-r--r--   0        0        0     1897 2023-06-04 10:45:57.994476 protocol0-1.0.13/protocol0/domain/lom/validation/ValidatorService.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.027208 protocol0-1.0.13/protocol0/domain/shared/__init__.py
--rw-r--r--   0        0        0     3720 2023-06-04 10:45:58.016585 protocol0-1.0.13/protocol0/domain/shared/ApplicationView.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.031631 protocol0-1.0.13/protocol0/domain/shared/backend/__init__.py
--rw-r--r--   0        0        0     1289 2023-06-04 11:46:25.602242 protocol0-1.0.13/protocol0/domain/shared/backend/Backend.py
--rw-r--r--   0        0        0      190 2023-06-04 10:45:58.029503 protocol0-1.0.13/protocol0/domain/shared/backend/BackendEvent.py
--rw-r--r--   0        0        0      103 2023-06-04 10:45:58.030619 protocol0-1.0.13/protocol0/domain/shared/backend/NotificationColorEnum.py
--rw-r--r--   0        0        0      644 2023-06-04 10:45:58.018432 protocol0-1.0.13/protocol0/domain/shared/BrowserServiceInterface.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.035738 protocol0-1.0.13/protocol0/domain/shared/errors/__init__.py
--rw-r--r--   0        0        0      605 2023-06-04 10:45:58.038272 protocol0-1.0.13/protocol0/domain/shared/errors/error_handler.py
--rw-r--r--   0        0        0      178 2023-06-04 10:45:58.033562 protocol0-1.0.13/protocol0/domain/shared/errors/ErrorRaisedEvent.py
--rw-r--r--   0        0        0       47 2023-06-04 10:45:58.034726 protocol0-1.0.13/protocol0/domain/shared/errors/Protocol0Error.py
--rw-r--r--   0        0        0      359 2023-06-04 10:45:58.035738 protocol0-1.0.13/protocol0/domain/shared/errors/Protocol0Warning.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.041860 protocol0-1.0.13/protocol0/domain/shared/event/__init__.py
--rw-r--r--   0        0        0     4775 2023-06-04 10:45:58.040274 protocol0-1.0.13/protocol0/domain/shared/event/DomainEventBus.py
--rw-r--r--   0        0        0      200 2023-06-04 10:45:58.040853 protocol0-1.0.13/protocol0/domain/shared/event/HasEmitter.py
--rw-r--r--   0        0        0      118 2023-06-04 10:45:58.020445 protocol0-1.0.13/protocol0/domain/shared/InterfaceClicksServiceInterface.py
--rw-r--r--   0        0        0      570 2023-06-04 10:45:58.021773 protocol0-1.0.13/protocol0/domain/shared/LiveObject.py
--rw-r--r--   0        0        0     1966 2023-06-04 10:45:58.022784 protocol0-1.0.13/protocol0/domain/shared/LiveObjectMapping.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.057489 protocol0-1.0.13/protocol0/domain/shared/scheduler/__init__.py
--rw-r--r--   0        0        0       42 2023-06-04 10:45:58.043249 protocol0-1.0.13/protocol0/domain/shared/scheduler/BarChangedEvent.py
--rw-r--r--   0        0        0       41 2023-06-04 10:45:58.045279 protocol0-1.0.13/protocol0/domain/shared/scheduler/BarEndingEvent.py
--rw-r--r--   0        0        0      309 2023-06-04 10:45:58.046880 protocol0-1.0.13/protocol0/domain/shared/scheduler/BeatSchedulerInterface.py
--rw-r--r--   0        0        0       46 2023-06-04 10:45:58.048660 protocol0-1.0.13/protocol0/domain/shared/scheduler/Last16thPassedEvent.py
--rw-r--r--   0        0        0       46 2023-06-04 10:45:58.049670 protocol0-1.0.13/protocol0/domain/shared/scheduler/Last32thPassedEvent.py
--rw-r--r--   0        0        0       45 2023-06-04 10:45:58.050669 protocol0-1.0.13/protocol0/domain/shared/scheduler/Last8thPassedEvent.py
--rw-r--r--   0        0        0       46 2023-06-04 10:45:58.051880 protocol0-1.0.13/protocol0/domain/shared/scheduler/LastBeatPassedEvent.py
--rw-r--r--   0        0        0     2550 2023-06-04 10:45:58.052927 protocol0-1.0.13/protocol0/domain/shared/scheduler/Scheduler.py
--rw-r--r--   0        0        0       47 2023-06-04 10:45:58.053931 protocol0-1.0.13/protocol0/domain/shared/scheduler/ThirdBeatPassedEvent.py
--rw-r--r--   0        0        0      130 2023-06-04 10:45:58.055529 protocol0-1.0.13/protocol0/domain/shared/scheduler/TickSchedulerEventInterface.py
--rw-r--r--   0        0        0      565 2023-06-04 10:45:58.056527 protocol0-1.0.13/protocol0/domain/shared/scheduler/TickSchedulerInterface.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.058511 protocol0-1.0.13/protocol0/domain/shared/script/__init__.py
--rw-r--r--   0        0        0      139 2023-06-04 10:45:58.023784 protocol0-1.0.13/protocol0/domain/shared/SessionServiceInterface.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.061074 protocol0-1.0.13/protocol0/domain/shared/ui/__init__.py
--rw-r--r--   0        0        0      128 2023-06-04 10:45:58.061074 protocol0-1.0.13/protocol0/domain/shared/ui/ColorEnum.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.062827 protocol0-1.0.13/protocol0/domain/shared/utils/__init__.py
--rw-r--r--   0        0        0      974 2023-06-04 10:45:58.064086 protocol0-1.0.13/protocol0/domain/shared/utils/concurrency.py
--rw-r--r--   0        0        0      924 2023-06-04 10:45:58.065095 protocol0-1.0.13/protocol0/domain/shared/utils/debug.py
--rw-r--r--   0        0        0     1607 2023-06-04 10:45:58.066096 protocol0-1.0.13/protocol0/domain/shared/utils/forward_to.py
--rw-r--r--   0        0        0     3223 2023-06-04 10:45:58.068405 protocol0-1.0.13/protocol0/domain/shared/utils/func.py
--rw-r--r--   0        0        0      270 2023-06-04 10:45:58.069412 protocol0-1.0.13/protocol0/domain/shared/utils/list.py
--rw-r--r--   0        0        0      545 2023-06-04 10:45:58.070414 protocol0-1.0.13/protocol0/domain/shared/utils/string.py
--rw-r--r--   0        0        0     4839 2023-06-04 10:45:58.071586 protocol0-1.0.13/protocol0/domain/shared/utils/timing.py
--rw-r--r--   0        0        0     3516 2023-06-04 10:45:58.073853 protocol0-1.0.13/protocol0/domain/shared/utils/utils.py
--rw-r--r--   0        0        0     2247 2023-06-04 10:45:58.024783 protocol0-1.0.13/protocol0/domain/shared/ValueScroller.py
--rw-r--r--   0        0        0     1003 2023-06-04 10:45:58.025785 protocol0-1.0.13/protocol0/domain/shared/ValueToggler.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.082256 protocol0-1.0.13/protocol0/domain/track_recorder/__init__.py
--rw-r--r--   0        0        0      687 2023-06-04 10:45:58.075832 protocol0-1.0.13/protocol0/domain/track_recorder/AbstractRecorderFactory.py
--rw-r--r--   0        0        0     3282 2023-06-04 10:45:58.076887 protocol0-1.0.13/protocol0/domain/track_recorder/BaseRecorder.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.086834 protocol0-1.0.13/protocol0/domain/track_recorder/config/__init__.py
--rw-r--r--   0        0        0     1809 2023-06-04 10:45:58.084242 protocol0-1.0.13/protocol0/domain/track_recorder/config/RecordConfig.py
--rw-r--r--   0        0        0     1202 2023-06-04 10:45:58.086292 protocol0-1.0.13/protocol0/domain/track_recorder/config/RecordProcessors.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.093102 protocol0-1.0.13/protocol0/domain/track_recorder/count_in/__init__.py
--rw-r--r--   0        0        0      412 2023-06-04 10:45:58.089216 protocol0-1.0.13/protocol0/domain/track_recorder/count_in/CountInInterface.py
--rw-r--r--   0        0        0     1663 2023-06-04 10:45:58.091089 protocol0-1.0.13/protocol0/domain/track_recorder/count_in/CountInOneBar.py
--rw-r--r--   0        0        0      645 2023-06-04 10:45:58.092101 protocol0-1.0.13/protocol0/domain/track_recorder/count_in/CountInShort.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.098582 protocol0-1.0.13/protocol0/domain/track_recorder/event/__init__.py
--rw-r--r--   0        0        0       47 2023-06-04 10:45:58.095096 protocol0-1.0.13/protocol0/domain/track_recorder/event/RecordCancelledEvent.py
--rw-r--r--   0        0        0       41 2023-06-04 10:45:58.096142 protocol0-1.0.13/protocol0/domain/track_recorder/event/RecordEndedEvent.py
--rw-r--r--   0        0        0      265 2023-06-04 10:45:58.098582 protocol0-1.0.13/protocol0/domain/track_recorder/event/RecordStartedEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.108560 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/__init__.py
--rw-r--r--   0        0        0       47 2023-06-04 10:45:58.100899 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/AudioClipSilentEvent.py
--rw-r--r--   0        0        0      265 2023-06-04 10:45:58.101897 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/ExtAudioRecordingEndedEvent.py
--rw-r--r--   0        0        0      267 2023-06-04 10:45:58.105102 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/ExtAudioRecordingStartedEvent.py
--rw-r--r--   0        0        0     3054 2023-06-04 10:45:58.106442 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/OnRecordEndClipTail.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.114071 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/__init__.py
--rw-r--r--   0        0        0     1958 2023-06-04 10:45:58.109961 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/PostRecordAudio.py
--rw-r--r--   0        0        0      994 2023-06-04 10:45:58.110916 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py
--rw-r--r--   0        0        0     1015 2023-06-04 10:45:58.113126 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/PreRecordAudio.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.117785 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/__init__.py
--rw-r--r--   0        0        0     2576 2023-06-04 10:45:58.116115 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py
--rw-r--r--   0        0        0     2191 2023-06-04 10:45:58.116779 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.123358 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_midi/__init__.py
--rw-r--r--   0        0        0     1491 2023-06-04 10:45:58.121310 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_midi/PostRecordMidi.py
--rw-r--r--   0        0        0      473 2023-06-04 10:45:58.122360 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_midi/PreRecordMidi.py
--rw-r--r--   0        0        0     4780 2023-06-04 10:45:58.107495 protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.128660 protocol0-1.0.13/protocol0/domain/track_recorder/recording_bar_length/__init__.py
--rw-r--r--   0        0        0      565 2023-06-04 10:45:58.124470 protocol0-1.0.13/protocol0/domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py
--rw-r--r--   0        0        0      890 2023-06-04 10:45:58.126481 protocol0-1.0.13/protocol0/domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py
--rw-r--r--   0        0        0       65 2023-06-04 10:45:58.128660 protocol0-1.0.13/protocol0/domain/track_recorder/recording_bar_length/SelectedRecordingBarLengthUpdatedEvent.py
--rw-r--r--   0        0        0      670 2023-06-04 10:45:58.079235 protocol0-1.0.13/protocol0/domain/track_recorder/RecordProcessorInterface.py
--rw-r--r--   0        0        0     7836 2023-06-04 10:45:58.081240 protocol0-1.0.13/protocol0/domain/track_recorder/RecordService.py
--rw-r--r--   0        0        0      897 2023-06-04 10:45:58.082256 protocol0-1.0.13/protocol0/domain/track_recorder/RecordTypeEnum.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.132602 protocol0-1.0.13/protocol0/domain/track_recorder/simple/__init__.py
--rw-r--r--   0        0        0      703 2023-06-04 10:45:58.130592 protocol0-1.0.13/protocol0/domain/track_recorder/simple/PostRecordSimple.py
--rw-r--r--   0        0        0     2240 2023-06-04 10:45:58.132602 protocol0-1.0.13/protocol0/domain/track_recorder/simple/RecorderSimpleFactory.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.133797 protocol0-1.0.13/protocol0/infra/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.141735 protocol0-1.0.13/protocol0/infra/interface/__init__.py
--rw-r--r--   0        0        0     5573 2023-06-04 10:45:58.137060 protocol0-1.0.13/protocol0/infra/interface/BrowserLoaderService.py
--rw-r--r--   0        0        0     2790 2023-06-04 10:45:58.138487 protocol0-1.0.13/protocol0/infra/interface/BrowserService.py
--rw-r--r--   0        0        0      427 2023-06-04 10:45:58.139987 protocol0-1.0.13/protocol0/infra/interface/InterfaceClicksService.py
--rw-r--r--   0        0        0      262 2023-06-04 10:45:58.140959 protocol0-1.0.13/protocol0/infra/interface/PixelEnum.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.145747 protocol0-1.0.13/protocol0/infra/interface/session/__init__.py
--rw-r--r--   0        0        0     2534 2023-06-04 10:45:58.143804 protocol0-1.0.13/protocol0/infra/interface/session/SessionService.py
--rw-r--r--   0        0        0      226 2023-06-04 10:45:58.144783 protocol0-1.0.13/protocol0/infra/interface/session/SessionUpdatedEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.147763 protocol0-1.0.13/protocol0/infra/logging/__init__.py
--rw-r--r--   0        0        0     2210 2023-06-04 10:45:58.146760 protocol0-1.0.13/protocol0/infra/logging/LoggerService.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.153445 protocol0-1.0.13/protocol0/infra/midi/__init__.py
--rw-r--r--   0        0        0      177 2023-06-04 10:45:58.148782 protocol0-1.0.13/protocol0/infra/midi/MidiBytesReceivedEvent.py
--rw-r--r--   0        0        0      173 2023-06-04 10:45:58.149808 protocol0-1.0.13/protocol0/infra/midi/MidiBytesSentEvent.py
--rw-r--r--   0        0        0     3279 2023-06-04 10:45:58.152441 protocol0-1.0.13/protocol0/infra/midi/MidiService.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.160342 protocol0-1.0.13/protocol0/infra/persistence/__init__.py
--rw-r--r--   0        0        0      254 2023-06-04 10:45:58.155275 protocol0-1.0.13/protocol0/infra/persistence/SongDataEnum.py
--rw-r--r--   0        0        0     3068 2023-06-04 10:45:58.157549 protocol0-1.0.13/protocol0/infra/persistence/SongDataService.py
--rw-r--r--   0        0        0     1229 2023-06-04 10:45:58.159336 protocol0-1.0.13/protocol0/infra/persistence/TrackData.py
--rw-r--r--   0        0        0      131 2023-06-04 10:45:58.160342 protocol0-1.0.13/protocol0/infra/persistence/TrackDataEnum.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.169857 protocol0-1.0.13/protocol0/infra/scheduler/__init__.py
--rw-r--r--   0        0        0     5140 2023-06-04 10:45:58.163172 protocol0-1.0.13/protocol0/infra/scheduler/BeatScheduler.py
--rw-r--r--   0        0        0      870 2023-06-04 10:45:58.164170 protocol0-1.0.13/protocol0/infra/scheduler/BeatSchedulerEvent.py
--rw-r--r--   0        0        0     3806 2023-06-04 10:45:58.166164 protocol0-1.0.13/protocol0/infra/scheduler/BeatTime.py
--rw-r--r--   0        0        0     2998 2023-06-04 10:45:58.167817 protocol0-1.0.13/protocol0/infra/scheduler/TickScheduler.py
--rw-r--r--   0        0        0     1031 2023-06-04 10:45:58.168904 protocol0-1.0.13/protocol0/infra/scheduler/TickSchedulerEvent.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.177847 protocol0-1.0.13/protocol0/shared/__init__.py
--rw-r--r--   0        0        0      813 2023-06-04 10:45:58.171851 protocol0-1.0.13/protocol0/shared/AbstractEnum.py
--rw-r--r--   0        0        0      935 2023-06-04 10:45:58.173857 protocol0-1.0.13/protocol0/shared/Config.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.185840 protocol0-1.0.13/protocol0/shared/logging/__init__.py
--rw-r--r--   0        0        0     1917 2023-06-04 10:45:58.182315 protocol0-1.0.13/protocol0/shared/logging/Logger.py
--rw-r--r--   0        0        0      271 2023-06-04 10:45:58.183812 protocol0-1.0.13/protocol0/shared/logging/LoggerServiceInterface.py
--rw-r--r--   0        0        0      154 2023-06-04 10:45:58.180268 protocol0-1.0.13/protocol0/shared/logging/LogLevelEnum.py
--rw-r--r--   0        0        0      724 2023-06-04 10:45:58.184859 protocol0-1.0.13/protocol0/shared/logging/StatusBar.py
--rw-r--r--   0        0        0     1048 2023-06-04 10:45:58.187481 protocol0-1.0.13/protocol0/shared/module.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.192173 protocol0-1.0.13/protocol0/shared/observer/__init__.py
--rw-r--r--   0        0        0      702 2023-06-04 10:45:58.190170 protocol0-1.0.13/protocol0/shared/observer/Observable.py
--rw-r--r--   0        0        0      259 2023-06-04 10:45:58.191217 protocol0-1.0.13/protocol0/shared/observer/Observer.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.251429 protocol0-1.0.13/protocol0/shared/sequence/__init__.py
--rw-r--r--   0        0        0      708 2023-06-04 10:45:58.202610 protocol0-1.0.13/protocol0/shared/sequence/HasSequenceState.py
--rw-r--r--   0        0        0     2073 2023-06-04 10:45:58.208602 protocol0-1.0.13/protocol0/shared/sequence/ParallelSequence.py
--rw-r--r--   0        0        0    12097 2023-06-04 10:45:58.216120 protocol0-1.0.13/protocol0/shared/sequence/Sequence.py
--rw-r--r--   0        0        0     1666 2023-06-04 10:45:58.226711 protocol0-1.0.13/protocol0/shared/sequence/SequenceState.py
--rw-r--r--   0        0        0     2859 2023-06-04 10:45:58.230723 protocol0-1.0.13/protocol0/shared/sequence/SequenceStep.py
--rw-r--r--   0        0        0      871 2023-06-04 10:45:58.239422 protocol0-1.0.13/protocol0/shared/sequence/SequenceTransition.py
--rw-r--r--   0        0        0     1801 2023-06-04 10:45:58.247419 protocol0-1.0.13/protocol0/shared/sequence/TimeoutLimit.py
--rw-r--r--   0        0        0    14062 2023-06-04 10:45:58.175834 protocol0-1.0.13/protocol0/shared/Song.py
--rw-r--r--   0        0        0      127 2023-06-04 10:45:58.257696 protocol0-1.0.13/protocol0/shared/types.py
--rw-r--r--   0        0        0      596 2023-06-04 10:45:58.176839 protocol0-1.0.13/protocol0/shared/UndoFacade.py
--rw-r--r--   0        0        0      230 2023-06-04 10:45:58.267194 protocol0-1.0.13/protocol0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.270276 protocol0-1.0.13/protocol0/tests/application/__init__.py
--rw-r--r--   0        0        0     2810 2023-06-04 10:45:58.277181 protocol0-1.0.13/protocol0/tests/application/test_multi_encoder.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.279877 protocol0-1.0.13/protocol0/tests/domain/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.288235 protocol0-1.0.13/protocol0/tests/domain/clip/__init__.py
--rw-r--r--   0        0        0      853 2023-06-04 10:45:58.291234 protocol0-1.0.13/protocol0/tests/domain/clip/test_clip_playing_position.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.293231 protocol0-1.0.13/protocol0/tests/domain/fixtures/__init__.py
--rw-r--r--   0        0        0     1017 2023-06-04 10:45:58.295525 protocol0-1.0.13/protocol0/tests/domain/fixtures/clip.py
--rw-r--r--   0        0        0      447 2023-06-04 10:45:58.296527 protocol0-1.0.13/protocol0/tests/domain/fixtures/clip_slot.py
--rw-r--r--   0        0        0       72 2023-06-04 10:45:58.298540 protocol0-1.0.13/protocol0/tests/domain/fixtures/clip_view.py
--rw-r--r--   0        0        0      261 2023-06-04 10:45:58.300169 protocol0-1.0.13/protocol0/tests/domain/fixtures/container.py
--rw-r--r--   0        0        0      665 2023-06-04 10:45:58.302297 protocol0-1.0.13/protocol0/tests/domain/fixtures/device.py
--rw-r--r--   0        0        0      319 2023-06-04 10:45:58.303346 protocol0-1.0.13/protocol0/tests/domain/fixtures/device_parameter.py
--rw-r--r--   0        0        0      872 2023-06-04 10:45:58.304365 protocol0-1.0.13/protocol0/tests/domain/fixtures/group_track.py
--rw-r--r--   0        0        0     2606 2023-06-04 10:45:58.306459 protocol0-1.0.13/protocol0/tests/domain/fixtures/p0.py
--rw-r--r--   0        0        0      264 2023-06-04 10:45:58.307497 protocol0-1.0.13/protocol0/tests/domain/fixtures/scene.py
--rw-r--r--   0        0        0     3057 2023-06-04 10:45:58.309517 protocol0-1.0.13/protocol0/tests/domain/fixtures/simple_track.py
--rw-r--r--   0        0        0     2731 2023-06-04 10:45:58.311536 protocol0-1.0.13/protocol0/tests/domain/fixtures/song.py
--rw-r--r--   0        0        0      308 2023-06-04 10:45:58.312968 protocol0-1.0.13/protocol0/tests/domain/fixtures/song_view.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.313964 protocol0-1.0.13/protocol0/tests/domain/scene/__init__.py
--rw-r--r--   0        0        0      587 2023-06-04 10:45:58.315489 protocol0-1.0.13/protocol0/tests/domain/scene/test_scene_clips.py
--rw-r--r--   0        0        0     1248 2023-06-04 10:45:58.317666 protocol0-1.0.13/protocol0/tests/domain/scene/test_scene_length.py
--rw-r--r--   0        0        0     1351 2023-06-04 10:45:58.320727 protocol0-1.0.13/protocol0/tests/domain/scene/test_scene_playing_position.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.321873 protocol0-1.0.13/protocol0/tests/domain/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.324109 protocol0-1.0.13/protocol0/tests/domain/shared/event/__init__.py
--rw-r--r--   0        0        0     1207 2023-06-04 10:45:58.326131 protocol0-1.0.13/protocol0/tests/domain/shared/event/test_domain_event_bus.py
--rw-r--r--   0        0        0      233 2023-06-04 10:45:58.328407 protocol0-1.0.13/protocol0/tests/domain/shared/test_decorators.py
--rw-r--r--   0        0        0      943 2023-06-04 10:45:58.329468 protocol0-1.0.13/protocol0/tests/domain/shared/test_live_object_mapping.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.331417 protocol0-1.0.13/protocol0/tests/domain/shared/utils/__init__.py
--rw-r--r--   0        0        0      607 2023-06-04 10:45:58.333484 protocol0-1.0.13/protocol0/tests/domain/shared/utils/test_func.py
--rw-r--r--   0        0        0     1477 2023-06-04 10:45:58.334483 protocol0-1.0.13/protocol0/tests/domain/shared/utils/test_utils.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.336489 protocol0-1.0.13/protocol0/tests/domain/track/__init__.py
--rw-r--r--   0        0        0      797 2023-06-04 10:45:58.338668 protocol0-1.0.13/protocol0/tests/domain/track/test_audio_to_midi_clip_mapping.py
--rw-r--r--   0        0        0      906 2023-06-04 10:45:58.339673 protocol0-1.0.13/protocol0/tests/domain/track/test_instantiation.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.342672 protocol0-1.0.13/protocol0/tests/domain/validation/__init__.py
--rw-r--r--   0        0        0     1379 2023-06-04 10:45:58.345219 protocol0-1.0.13/protocol0/tests/domain/validation/test_aggregate_validator.py
--rw-r--r--   0        0        0     1031 2023-06-04 10:45:58.347067 protocol0-1.0.13/protocol0/tests/domain/validation/test_callback_validator.py
--rw-r--r--   0        0        0     1086 2023-06-04 10:45:58.350417 protocol0-1.0.13/protocol0/tests/domain/validation/test_property_validator.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.351476 protocol0-1.0.13/protocol0/tests/infra/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.353740 protocol0-1.0.13/protocol0/tests/infra/listeners/__init__.py
--rw-r--r--   0        0        0     1301 2023-06-04 10:45:58.355876 protocol0-1.0.13/protocol0/tests/infra/listeners/test_subject_slot.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.361461 protocol0-1.0.13/protocol0/tests/infra/scheduler/__init__.py
--rw-r--r--   0        0        0      504 2023-06-04 10:45:58.358766 protocol0-1.0.13/protocol0/tests/infra/scheduler/TickSchedulerEventTest.py
--rw-r--r--   0        0        0      765 2023-06-04 10:45:58.360463 protocol0-1.0.13/protocol0/tests/infra/scheduler/TickSchedulerTest.py
--rw-r--r--   0        0        0     1978 2023-06-04 10:45:58.364768 protocol0-1.0.13/protocol0/tests/infra/test_scheduler.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.366760 protocol0-1.0.13/protocol0/tests/shared/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 10:45:58.368734 protocol0-1.0.13/protocol0/tests/shared/sequence/__init__.py
--rw-r--r--   0        0        0     1415 2023-06-04 10:45:58.370802 protocol0-1.0.13/protocol0/tests/shared/sequence/test_sanity_sequence.py
--rw-r--r--   0        0        0     3330 2023-06-04 10:45:58.372490 protocol0-1.0.13/protocol0/tests/shared/sequence/test_sequence.py
--rw-r--r--   0        0        0     1712 2023-06-04 10:45:58.374260 protocol0-1.0.13/protocol0/tests/shared/sequence/test_sequence_parallel.py
--rw-r--r--   0        0        0      565 2023-06-04 10:45:58.376262 protocol0-1.0.13/protocol0/tests/shared/test_container.py
--rw-r--r--   0        0        0     1780 2023-06-04 14:32:20.185629 protocol0-1.0.13/pyproject.toml
--rw-r--r--   0        0        0     5919 2023-06-04 12:13:42.155521 protocol0-1.0.13/README.md
--rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 protocol0-1.0.13/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-06-04 10:45:57.549172 protocol0-1.0.15/LICENSE.md
+-rw-r--r--   0        0        0      390 2023-06-04 21:50:08.618369 protocol0-1.0.15/protocol0/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.565833 protocol0-1.0.15/protocol0/application/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.605682 protocol0-1.0.15/protocol0/application/command/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-04 10:45:57.567447 protocol0-1.0.15/protocol0/application/command/BounceTrackToAudioCommand.py
+-rw-r--r--   0        0        0      155 2023-06-04 10:45:57.568433 protocol0-1.0.15/protocol0/application/command/CheckAudioExportValidCommand.py
+-rw-r--r--   0        0        0      151 2023-06-04 10:45:57.570579 protocol0-1.0.15/protocol0/application/command/DrumRackToSimplerCommand.py
+-rw-r--r--   0        0        0      356 2023-06-04 10:45:57.571591 protocol0-1.0.15/protocol0/application/command/EmitBackendEventCommand.py
+-rw-r--r--   0        0        0      356 2023-06-04 10:45:57.572591 protocol0-1.0.15/protocol0/application/command/FireSceneToPositionCommand.py
+-rw-r--r--   0        0        0      151 2023-06-04 10:45:57.573707 protocol0-1.0.15/protocol0/application/command/FireSelectedSceneCommand.py
+-rw-r--r--   0        0        0      145 2023-06-04 10:45:57.573707 protocol0-1.0.15/protocol0/application/command/GetSetStateCommand.py
+-rw-r--r--   0        0        0      148 2023-06-04 10:45:57.574719 protocol0-1.0.15/protocol0/application/command/GoToGroupTrackCommand.py
+-rw-r--r--   0        0        0      288 2023-06-04 10:45:57.575761 protocol0-1.0.15/protocol0/application/command/LoadDeviceCommand.py
+-rw-r--r--   0        0        0      389 2023-06-04 10:45:57.576774 protocol0-1.0.15/protocol0/application/command/LoadDrumRackCommand.py
+-rw-r--r--   0        0        0      151 2023-06-04 10:45:57.577813 protocol0-1.0.15/protocol0/application/command/LoadMatchingTrackCommand.py
+-rw-r--r--   0        0        0      146 2023-06-04 10:45:57.579832 protocol0-1.0.15/protocol0/application/command/LoadMinitaurCommand.py
+-rw-r--r--   0        0        0      142 2023-06-04 10:45:57.580882 protocol0-1.0.15/protocol0/application/command/LoadRev2Command.py
+-rw-r--r--   0        0        0      315 2023-06-04 10:45:57.581884 protocol0-1.0.15/protocol0/application/command/MidiNoteCommand.py
+-rw-r--r--   0        0        0      147 2023-06-04 10:45:57.583845 protocol0-1.0.15/protocol0/application/command/PlayPauseSongCommand.py
+-rw-r--r--   0        0        0      149 2023-06-04 10:45:57.584884 protocol0-1.0.15/protocol0/application/command/RecordUnlimitedCommand.py
+-rw-r--r--   0        0        0      146 2023-06-04 10:45:57.586900 protocol0-1.0.15/protocol0/application/command/ReloadScriptCommand.py
+-rw-r--r--   0        0        0      147 2023-06-04 10:45:57.587909 protocol0-1.0.15/protocol0/application/command/ResetPlaybackCommand.py
+-rw-r--r--   0        0        0      519 2023-06-04 21:57:42.593211 protocol0-1.0.15/protocol0/application/command/ScrollScenePositionCommand.py
+-rw-r--r--   0        0        0      293 2023-06-04 10:45:57.590035 protocol0-1.0.15/protocol0/application/command/ScrollScenesCommand.py
+-rw-r--r--   0        0        0      303 2023-06-04 10:45:57.590035 protocol0-1.0.15/protocol0/application/command/ScrollSceneTracksCommand.py
+-rw-r--r--   0        0        0      303 2023-06-04 10:45:57.592072 protocol0-1.0.15/protocol0/application/command/ScrollTrackVolumeCommand.py
+-rw-r--r--   0        0        0      310 2023-06-04 10:45:57.593196 protocol0-1.0.15/protocol0/application/command/SelectOrLoadDeviceCommand.py
+-rw-r--r--   0        0        0      293 2023-06-04 21:57:42.603211 protocol0-1.0.15/protocol0/application/command/SelectTrackCommand.py
+-rw-r--r--   0        0        0     1641 2023-06-04 10:45:57.595240 protocol0-1.0.15/protocol0/application/command/SerializableCommand.py
+-rw-r--r--   0        0        0      297 2023-06-04 10:45:57.596985 protocol0-1.0.15/protocol0/application/command/ShowAutomationCommand.py
+-rw-r--r--   0        0        0      148 2023-06-04 10:45:57.597931 protocol0-1.0.15/protocol0/application/command/ShowInstrumentCommand.py
+-rw-r--r--   0        0        0      284 2023-06-04 10:45:57.598925 protocol0-1.0.15/protocol0/application/command/ShowMessageCommand.py
+-rw-r--r--   0        0        0      143 2023-06-04 10:45:57.599929 protocol0-1.0.15/protocol0/application/command/ToggleArmCommand.py
+-rw-r--r--   0        0        0      145 2023-06-04 10:45:57.600679 protocol0-1.0.15/protocol0/application/command/ToggleNotesCommand.py
+-rw-r--r--   0        0        0      154 2023-06-04 10:45:57.601689 protocol0-1.0.15/protocol0/application/command/ToggleReferenceTrackCommand.py
+-rw-r--r--   0        0        0      149 2023-06-04 10:45:57.603768 protocol0-1.0.15/protocol0/application/command/ToggleSceneLoopCommand.py
+-rw-r--r--   0        0        0      153 2023-06-04 10:45:57.604688 protocol0-1.0.15/protocol0/application/command/UnfoldSelectedSceneCommand.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.646726 protocol0-1.0.15/protocol0/application/command_handler/__init__.py
+-rw-r--r--   0        0        0      543 2023-06-04 21:57:42.639576 protocol0-1.0.15/protocol0/application/command_handler/BounceTrackToAudioCommandHandler.py
+-rw-r--r--   0        0        0      850 2023-06-04 21:57:42.668208 protocol0-1.0.15/protocol0/application/command_handler/CheckAudioExportValidCommandHandler.py
+-rw-r--r--   0        0        0      443 2023-06-04 10:45:57.610241 protocol0-1.0.15/protocol0/application/command_handler/CommandHandlerInterface.py
+-rw-r--r--   0        0        0      542 2023-06-04 10:45:57.612239 protocol0-1.0.15/protocol0/application/command_handler/DrumRackToSimplerCommandHandler.py
+-rw-r--r--   0        0        0      568 2023-06-04 10:45:57.612626 protocol0-1.0.15/protocol0/application/command_handler/EmitBackendEventCommandHandler.py
+-rw-r--r--   0        0        0     1918 2023-06-04 10:45:57.613873 protocol0-1.0.15/protocol0/application/command_handler/FireSceneToPositionCommandHandler.py
+-rw-r--r--   0        0        0      546 2023-06-04 10:45:57.615884 protocol0-1.0.15/protocol0/application/command_handler/FireSelectedSceneCommandHandler.py
+-rw-r--r--   0        0        0      435 2023-06-04 10:45:57.616870 protocol0-1.0.15/protocol0/application/command_handler/GetSetStateCommandHandler.py
+-rw-r--r--   0        0        0      456 2023-06-04 10:45:57.618217 protocol0-1.0.15/protocol0/application/command_handler/GoToGroupTrackCommandHandler.py
+-rw-r--r--   0        0        0      529 2023-06-04 10:45:57.619187 protocol0-1.0.15/protocol0/application/command_handler/LoadDeviceCommandHandler.py
+-rw-r--r--   0        0        0      728 2023-06-04 21:57:42.697208 protocol0-1.0.15/protocol0/application/command_handler/LoadDrumRackCommandHandler.py
+-rw-r--r--   0        0        0      543 2023-06-04 10:45:57.621185 protocol0-1.0.15/protocol0/application/command_handler/LoadMatchingTrackCommandHandler.py
+-rw-r--r--   0        0        0      557 2023-06-04 10:45:57.622862 protocol0-1.0.15/protocol0/application/command_handler/LoadMinitaurCommandHandler.py
+-rw-r--r--   0        0        0      529 2023-06-04 10:45:57.622862 protocol0-1.0.15/protocol0/application/command_handler/LoadRev2CommandHandler.py
+-rw-r--r--   0        0        0     1641 2023-06-04 10:45:57.624221 protocol0-1.0.15/protocol0/application/command_handler/MidiNoteCommandHandler.py
+-rw-r--r--   0        0        0      483 2023-06-04 10:45:57.625823 protocol0-1.0.15/protocol0/application/command_handler/PlayPauseSongCommandHandler.py
+-rw-r--r--   0        0        0      670 2023-06-04 10:45:57.627331 protocol0-1.0.15/protocol0/application/command_handler/RecordUnlimitedCommandHandler.py
+-rw-r--r--   0        0        0      796 2023-06-04 10:45:57.628329 protocol0-1.0.15/protocol0/application/command_handler/ReloadScriptCommandHandler.py
+-rw-r--r--   0        0        0      465 2023-06-04 10:45:57.628778 protocol0-1.0.15/protocol0/application/command_handler/ResetPlaybackCommandHandler.py
+-rw-r--r--   0        0        0      590 2023-06-04 10:45:57.630529 protocol0-1.0.15/protocol0/application/command_handler/ScrollScenePositionCommandHandler.py
+-rw-r--r--   0        0        0      481 2023-06-04 10:45:57.632529 protocol0-1.0.15/protocol0/application/command_handler/ScrollScenesCommandHandler.py
+-rw-r--r--   0        0        0      447 2023-06-04 10:45:57.631529 protocol0-1.0.15/protocol0/application/command_handler/ScrollSceneTracksCommandHandler.py
+-rw-r--r--   0        0        0      457 2023-06-04 10:45:57.633529 protocol0-1.0.15/protocol0/application/command_handler/ScrollTrackVolumeCommandHandler.py
+-rw-r--r--   0        0        0      614 2023-06-04 10:45:57.635122 protocol0-1.0.15/protocol0/application/command_handler/SelectOrLoadDeviceCommandHandler.py
+-rw-r--r--   0        0        0      611 2023-06-04 10:45:57.636852 protocol0-1.0.15/protocol0/application/command_handler/SelectTrackCommandHandler.py
+-rw-r--r--   0        0        0      505 2023-06-04 10:45:57.637892 protocol0-1.0.15/protocol0/application/command_handler/ShowAutomationCommandHandler.py
+-rw-r--r--   0        0        0      555 2023-06-04 10:45:57.638900 protocol0-1.0.15/protocol0/application/command_handler/ShowInstrumentCommandHandler.py
+-rw-r--r--   0        0        0      428 2023-06-04 10:45:57.640471 protocol0-1.0.15/protocol0/application/command_handler/ShowMessageCommandHandler.py
+-rw-r--r--   0        0        0      505 2023-06-04 10:45:57.641521 protocol0-1.0.15/protocol0/application/command_handler/ToggleArmCommandJHandler.py
+-rw-r--r--   0        0        0      400 2023-06-04 10:45:57.642495 protocol0-1.0.15/protocol0/application/command_handler/ToggleNotesCommandHandler.py
+-rw-r--r--   0        0        0      432 2023-06-04 10:45:57.643503 protocol0-1.0.15/protocol0/application/command_handler/ToggleReferenceTrackCommandHandler.py
+-rw-r--r--   0        0        0      487 2023-06-04 10:45:57.644480 protocol0-1.0.15/protocol0/application/command_handler/ToggleSceneLoopCommandHandler.py
+-rw-r--r--   0        0        0      427 2023-06-04 10:45:57.646726 protocol0-1.0.15/protocol0/application/command_handler/UnfoldSelectedSceneCommandHandler.py
+-rw-r--r--   0        0        0     4453 2023-06-04 10:45:57.557129 protocol0-1.0.15/protocol0/application/CommandBus.py
+-rw-r--r--   0        0        0     1420 2023-06-04 10:45:57.558132 protocol0-1.0.15/protocol0/application/CommandBusHistory.py
+-rw-r--r--   0        0        0    13004 2023-06-04 21:57:43.510161 protocol0-1.0.15/protocol0/application/Container.py
+-rw-r--r--   0        0        0      196 2023-06-04 10:45:57.561438 protocol0-1.0.15/protocol0/application/ContainerInterface.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.655439 protocol0-1.0.15/protocol0/application/control_surface/__init__.py
+-rw-r--r--   0        0        0      772 2023-06-04 10:45:57.648426 protocol0-1.0.15/protocol0/application/control_surface/ActionGroupFactory.py
+-rw-r--r--   0        0        0     2752 2023-06-04 21:57:42.864210 protocol0-1.0.15/protocol0/application/control_surface/ActionGroupInterface.py
+-rw-r--r--   0        0        0     2983 2023-06-04 10:45:57.652338 protocol0-1.0.15/protocol0/application/control_surface/EncoderAction.py
+-rw-r--r--   0        0        0      173 2023-06-04 10:45:57.653434 protocol0-1.0.15/protocol0/application/control_surface/EncoderMoveEnum.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.665941 protocol0-1.0.15/protocol0/application/control_surface/group/__init__.py
+-rw-r--r--   0        0        0     1356 2023-06-04 10:45:57.656442 protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupClip.py
+-rw-r--r--   0        0        0     1268 2023-06-04 10:45:57.657549 protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupCut.py
+-rw-r--r--   0        0        0      860 2023-06-04 21:57:42.813212 protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupFix.py
+-rw-r--r--   0        0        0     1240 2023-06-04 10:45:57.660938 protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupLog.py
+-rw-r--r--   0        0        0     3967 2023-06-04 21:57:43.062898 protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupMain.py
+-rw-r--r--   0        0        0      595 2023-06-04 10:45:57.662946 protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupSample.py
+-rw-r--r--   0        0        0      985 2023-06-04 10:45:57.663984 protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupSet.py
+-rw-r--r--   0        0        0     2122 2023-06-04 21:57:42.925218 protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupTest.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.667947 protocol0-1.0.15/protocol0/application/control_surface/group/legacy/__init__.py
+-rw-r--r--   0        0        0     1090 2023-06-04 10:45:57.666989 protocol0-1.0.15/protocol0/application/control_surface/group/legacy/ActionGroupPreset.py
+-rw-r--r--   0        0        0     5488 2023-06-04 10:45:57.654464 protocol0-1.0.15/protocol0/application/control_surface/MultiEncoder.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.671223 protocol0-1.0.15/protocol0/application/error/__init__.py
+-rw-r--r--   0        0        0     6184 2023-06-04 21:55:34.092786 protocol0-1.0.15/protocol0/application/error/ErrorService.py
+-rw-r--r--   0        0        0      370 2023-06-04 10:45:57.672260 protocol0-1.0.15/protocol0/application/main.py
+-rw-r--r--   0        0        0     2029 2023-06-04 16:30:25.923334 protocol0-1.0.15/protocol0/application/Protocol0.py
+-rw-r--r--   0        0        0     1884 2023-06-04 21:57:42.932210 protocol0-1.0.15/protocol0/application/Protocol0Midi.py
+-rw-r--r--   0        0        0       64 2023-06-04 10:45:57.679519 protocol0-1.0.15/protocol0/application/push2/__init__.py
+-rw-r--r--   0        0        0     5916 2023-06-04 10:45:57.673855 protocol0-1.0.15/protocol0/application/push2/P0Push2.py
+-rw-r--r--   0        0        0     4102 2023-06-04 21:57:43.085900 protocol0-1.0.15/protocol0/application/push2/P0SessionRingTrackProvider.py
+-rw-r--r--   0        0        0      678 2023-06-04 10:45:57.676182 protocol0-1.0.15/protocol0/application/push2/P0ShowInstrumentMode.py
+-rw-r--r--   0        0        0      575 2023-06-04 10:45:57.677560 protocol0-1.0.15/protocol0/application/push2/P0TrackListComponent.py
+-rw-r--r--   0        0        0      476 2023-06-04 10:45:57.678518 protocol0-1.0.15/protocol0/application/push2/P0TransportComponent.py
+-rw-r--r--   0        0        0       50 2023-06-04 10:45:57.564805 protocol0-1.0.15/protocol0/application/ScriptDisconnectedEvent.py
+-rw-r--r--   0        0        0       52 2023-06-04 10:45:57.565833 protocol0-1.0.15/protocol0/application/ScriptResetActivatedEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.680523 protocol0-1.0.15/protocol0/domain/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.690394 protocol0-1.0.15/protocol0/domain/audit/__init__.py
+-rw-r--r--   0        0        0     4919 2023-06-04 21:57:43.534159 protocol0-1.0.15/protocol0/domain/audit/AudioLatencyAnalyzerService.py
+-rw-r--r--   0        0        0     8658 2023-06-04 21:57:43.549158 protocol0-1.0.15/protocol0/domain/audit/LogService.py
+-rw-r--r--   0        0        0     1357 2023-06-04 21:57:42.946210 protocol0-1.0.15/protocol0/domain/audit/LOMAnalyzerService.py
+-rw-r--r--   0        0        0     2353 2023-06-04 21:57:43.053898 protocol0-1.0.15/protocol0/domain/audit/SetFixerService.py
+-rw-r--r--   0        0        0     3309 2023-06-04 10:45:57.689152 protocol0-1.0.15/protocol0/domain/audit/SetUpgradeService.py
+-rw-r--r--   0        0        0      412 2023-06-04 10:45:57.690321 protocol0-1.0.15/protocol0/domain/audit/SongStatsService.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.701613 protocol0-1.0.15/protocol0/domain/audit/stats/__init__.py
+-rw-r--r--   0        0        0     1429 2023-06-04 10:45:57.691947 protocol0-1.0.15/protocol0/domain/audit/stats/ClipStats.py
+-rw-r--r--   0        0        0     3331 2023-06-04 21:57:43.194631 protocol0-1.0.15/protocol0/domain/audit/stats/DeviceStats.py
+-rw-r--r--   0        0        0     2275 2023-06-04 10:45:57.695016 protocol0-1.0.15/protocol0/domain/audit/stats/SampleStats.py
+-rw-r--r--   0        0        0     1014 2023-06-04 10:45:57.696600 protocol0-1.0.15/protocol0/domain/audit/stats/SceneStats.py
+-rw-r--r--   0        0        0      995 2023-06-04 10:45:57.698627 protocol0-1.0.15/protocol0/domain/audit/stats/SongStats.py
+-rw-r--r--   0        0        0      180 2023-06-04 10:45:57.699612 protocol0-1.0.15/protocol0/domain/audit/stats/Stats.py
+-rw-r--r--   0        0        0      900 2023-06-04 10:45:57.700613 protocol0-1.0.15/protocol0/domain/audit/stats/TrackStats.py
+-rw-r--r--   0        0        0      337 2023-06-04 10:45:57.702662 protocol0-1.0.15/protocol0/domain/audit/utils.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.703673 protocol0-1.0.15/protocol0/domain/lom/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.721607 protocol0-1.0.15/protocol0/domain/lom/clip/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-04 10:45:57.705981 protocol0-1.0.15/protocol0/domain/lom/clip/AudioClip.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.725393 protocol0-1.0.15/protocol0/domain/lom/clip/automation/__init__.py
+-rw-r--r--   0        0        0     3719 2023-06-04 10:45:57.723658 protocol0-1.0.15/protocol0/domain/lom/clip/automation/ClipAutomation.py
+-rw-r--r--   0        0        0     1888 2023-06-04 10:45:57.724335 protocol0-1.0.15/protocol0/domain/lom/clip/automation/ClipAutomationEnvelope.py
+-rw-r--r--   0        0        0     7866 2023-06-04 10:45:57.707359 protocol0-1.0.15/protocol0/domain/lom/clip/Clip.py
+-rw-r--r--   0        0        0      913 2023-06-04 10:45:57.708370 protocol0-1.0.15/protocol0/domain/lom/clip/ClipAppearance.py
+-rw-r--r--   0        0        0      160 2023-06-04 10:45:57.709373 protocol0-1.0.15/protocol0/domain/lom/clip/ClipColorEnum.py
+-rw-r--r--   0        0        0      183 2023-06-04 10:45:57.710394 protocol0-1.0.15/protocol0/domain/lom/clip/ClipConfig.py
+-rw-r--r--   0        0        0      287 2023-06-04 10:45:57.711366 protocol0-1.0.15/protocol0/domain/lom/clip/ClipCreatedOrDeletedEvent.py
+-rw-r--r--   0        0        0       50 2023-06-04 10:45:57.713367 protocol0-1.0.15/protocol0/domain/lom/clip/ClipEnvelopeShowedEvent.py
+-rw-r--r--   0        0        0     4296 2023-06-04 21:57:43.361630 protocol0-1.0.15/protocol0/domain/lom/clip/ClipInfo.py
+-rw-r--r--   0        0        0     5558 2023-06-04 10:45:57.714893 protocol0-1.0.15/protocol0/domain/lom/clip/ClipLoop.py
+-rw-r--r--   0        0        0     4087 2023-06-04 10:45:57.716003 protocol0-1.0.15/protocol0/domain/lom/clip/ClipName.py
+-rw-r--r--   0        0        0      921 2023-06-04 21:57:43.123896 protocol0-1.0.15/protocol0/domain/lom/clip/ClipPlayingPosition.py
+-rw-r--r--   0        0        0      192 2023-06-04 10:45:57.718013 protocol0-1.0.15/protocol0/domain/lom/clip/ClipSlotSelectedEvent.py
+-rw-r--r--   0        0        0     2093 2023-06-04 21:57:43.195629 protocol0-1.0.15/protocol0/domain/lom/clip/ClipTail.py
+-rw-r--r--   0        0        0     7368 2023-06-04 10:45:57.721102 protocol0-1.0.15/protocol0/domain/lom/clip/MidiClip.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.736330 protocol0-1.0.15/protocol0/domain/lom/clip_slot/__init__.py
+-rw-r--r--   0        0        0     2644 2023-06-04 10:45:57.728387 protocol0-1.0.15/protocol0/domain/lom/clip_slot/AudioClipSlot.py
+-rw-r--r--   0        0        0     5707 2023-06-04 21:57:43.516158 protocol0-1.0.15/protocol0/domain/lom/clip_slot/ClipSlot.py
+-rw-r--r--   0        0        0      736 2023-06-04 10:45:57.730448 protocol0-1.0.15/protocol0/domain/lom/clip_slot/ClipSlotAppearance.py
+-rw-r--r--   0        0        0      173 2023-06-04 21:57:43.098897 protocol0-1.0.15/protocol0/domain/lom/clip_slot/ClipSlotHasClipEvent.py
+-rw-r--r--   0        0        0      401 2023-06-04 10:45:57.734375 protocol0-1.0.15/protocol0/domain/lom/clip_slot/MidiClipSlot.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.763299 protocol0-1.0.15/protocol0/domain/lom/device/__init__.py
+-rw-r--r--   0        0        0     4723 2023-06-04 21:57:43.387627 protocol0-1.0.15/protocol0/domain/lom/device/Device.py
+-rw-r--r--   0        0        0     1445 2023-06-04 10:45:57.739369 protocol0-1.0.15/protocol0/domain/lom/device/DeviceChain.py
+-rw-r--r--   0        0        0     6824 2023-06-04 21:57:43.582156 protocol0-1.0.15/protocol0/domain/lom/device/DeviceDisplayService.py
+-rw-r--r--   0        0        0    12713 2023-06-04 10:45:57.742747 protocol0-1.0.15/protocol0/domain/lom/device/DeviceEnum.py
+-rw-r--r--   0        0        0      548 2023-06-04 21:57:43.203626 protocol0-1.0.15/protocol0/domain/lom/device/DeviceEnumGroup.py
+-rw-r--r--   0        0        0      217 2023-06-04 10:45:57.744759 protocol0-1.0.15/protocol0/domain/lom/device/DeviceLoadedEvent.py
+-rw-r--r--   0        0        0     4628 2023-06-04 10:45:57.745872 protocol0-1.0.15/protocol0/domain/lom/device/DeviceService.py
+-rw-r--r--   0        0        0     2190 2023-06-04 21:57:43.346630 protocol0-1.0.15/protocol0/domain/lom/device/DrumPad.py
+-rw-r--r--   0        0        0     1193 2023-06-04 10:45:57.748925 protocol0-1.0.15/protocol0/domain/lom/device/DrumRackDevice.py
+-rw-r--r--   0        0        0       46 2023-06-04 10:45:57.749925 protocol0-1.0.15/protocol0/domain/lom/device/DrumRackLoadedEvent.py
+-rw-r--r--   0        0        0     1607 2023-06-04 21:57:43.315625 protocol0-1.0.15/protocol0/domain/lom/device/DrumRackSampleService.py
+-rw-r--r--   0        0        0     7283 2023-06-04 21:53:53.078844 protocol0-1.0.15/protocol0/domain/lom/device/DrumRackService.py
+-rw-r--r--   0        0        0     1345 2023-06-04 21:57:43.330627 protocol0-1.0.15/protocol0/domain/lom/device/MixerDevice.py
+-rw-r--r--   0        0        0     1290 2023-06-04 10:45:57.755801 protocol0-1.0.15/protocol0/domain/lom/device/PluginDevice.py
+-rw-r--r--   0        0        0     1822 2023-06-04 10:45:57.756778 protocol0-1.0.15/protocol0/domain/lom/device/RackDevice.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.760401 protocol0-1.0.15/protocol0/domain/lom/device/Sample/__init__.py
+-rw-r--r--   0        0        0     1419 2023-06-04 10:45:57.758833 protocol0-1.0.15/protocol0/domain/lom/device/Sample/Sample.py
+-rw-r--r--   0        0        0      346 2023-06-04 10:45:57.759368 protocol0-1.0.15/protocol0/domain/lom/device/Sample/SampleNotFoundError.py
+-rw-r--r--   0        0        0     1796 2023-06-04 21:53:17.809611 protocol0-1.0.15/protocol0/domain/lom/device/SimplerDevice.py
+-rw-r--r--   0        0        0     5436 2023-06-04 10:45:57.761219 protocol0-1.0.15/protocol0/domain/lom/device/SimpleTrackDevices.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.771500 protocol0-1.0.15/protocol0/domain/lom/device_parameter/__init__.py
+-rw-r--r--   0        0        0     4605 2023-06-04 21:57:43.796220 protocol0-1.0.15/protocol0/domain/lom/device_parameter/DeviceParameter.py
+-rw-r--r--   0        0        0     4124 2023-06-04 10:45:57.767305 protocol0-1.0.15/protocol0/domain/lom/device_parameter/DeviceParameterEnum.py
+-rw-r--r--   0        0        0      925 2023-06-04 10:45:57.770075 protocol0-1.0.15/protocol0/domain/lom/device_parameter/DeviceParameterValue.py
+-rw-r--r--   0        0        0     1431 2023-06-04 10:45:57.771500 protocol0-1.0.15/protocol0/domain/lom/device_parameter/LinkedDeviceParameters.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.780156 protocol0-1.0.15/protocol0/domain/lom/instrument/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.794364 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-04 10:45:57.782374 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentAddictiveKeys.py
+-rw-r--r--   0        0        0      500 2023-06-04 10:45:57.784360 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentDrumRack.py
+-rw-r--r--   0        0        0      394 2023-06-04 10:45:57.786341 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentKontakt.py
+-rw-r--r--   0        0        0      737 2023-06-04 10:45:57.787353 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentMinitaur.py
+-rw-r--r--   0        0        0      382 2023-06-04 10:45:57.788367 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentOpus.py
+-rw-r--r--   0        0        0      382 2023-06-04 10:45:57.789389 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentPlay.py
+-rw-r--r--   0        0        0     2970 2023-06-04 21:57:43.594158 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentRev2.py
+-rw-r--r--   0        0        0      290 2023-06-04 10:45:57.791347 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentSampler.py
+-rw-r--r--   0        0        0      505 2023-06-04 10:45:57.792383 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentSerum.py
+-rw-r--r--   0        0        0     1013 2023-06-04 10:45:57.793339 protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentSimpler.py
+-rw-r--r--   0        0        0      252 2023-06-04 10:45:57.773816 protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentActivatedEvent.py
+-rw-r--r--   0        0        0      235 2023-06-04 10:45:57.774819 protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentColorEnum.py
+-rw-r--r--   0        0        0     4503 2023-06-04 21:57:43.628157 protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentDisplayService.py
+-rw-r--r--   0        0        0     4273 2023-06-04 10:45:57.778152 protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentFactory.py
+-rw-r--r--   0        0        0     4478 2023-06-04 21:57:44.031221 protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentInterface.py
+-rw-r--r--   0        0        0       50 2023-06-04 10:45:57.780156 protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentSelectedEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.803314 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/__init__.py
+-rw-r--r--   0        0        0      956 2023-06-04 10:45:57.795457 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/InstrumentPreset.py
+-rw-r--r--   0        0        0     3209 2023-06-04 10:45:57.797324 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/InstrumentPresetList.py
+-rw-r--r--   0        0        0     1957 2023-06-04 10:45:57.799353 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/InstrumentPresetScrollerService.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.811182 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_changer/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-04 10:45:57.804773 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py
+-rw-r--r--   0        0        0      498 2023-06-04 10:45:57.806804 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_changer/PresetChangerInterface.py
+-rw-r--r--   0        0        0      811 2023-06-04 10:45:57.809166 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py
+-rw-r--r--   0        0        0      581 2023-06-04 10:45:57.810171 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.820462 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/__init__.py
+-rw-r--r--   0        0        0     1982 2023-06-04 10:45:57.812607 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py
+-rw-r--r--   0        0        0      613 2023-06-04 10:45:57.813619 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/FilePresetImporter.py
+-rw-r--r--   0        0        0      387 2023-06-04 10:45:57.815883 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/NullPresetImporter.py
+-rw-r--r--   0        0        0      699 2023-06-04 10:45:57.816260 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py
+-rw-r--r--   0        0        0     1858 2023-06-04 21:57:43.569159 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py
+-rw-r--r--   0        0        0      812 2023-06-04 10:45:57.818271 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/PresetImportInterface.py
+-rw-r--r--   0        0        0      686 2023-06-04 10:45:57.820462 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.825961 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_initializer/__init__.py
+-rw-r--r--   0        0        0      627 2023-06-04 10:45:57.822498 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py
+-rw-r--r--   0        0        0      575 2023-06-04 10:45:57.823914 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py
+-rw-r--r--   0        0        0      611 2023-06-04 10:45:57.824959 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py
+-rw-r--r--   0        0        0      171 2023-06-04 10:45:57.800351 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/PresetDisplayOptionEnum.py
+-rw-r--r--   0        0        0      155 2023-06-04 10:45:57.801397 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/PresetProgramSelectedEvent.py
+-rw-r--r--   0        0        0      145 2023-06-04 10:45:57.803314 protocol0-1.0.15/protocol0/domain/lom/instrument/preset/SampleSelectedEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.827732 protocol0-1.0.15/protocol0/domain/lom/loop/__init__.py
+-rw-r--r--   0        0        0      915 2023-06-04 10:45:57.827732 protocol0-1.0.15/protocol0/domain/lom/loop/LoopableInterface.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.830739 protocol0-1.0.15/protocol0/domain/lom/note/__init__.py
+-rw-r--r--   0        0        0     3539 2023-06-04 21:57:43.828221 protocol0-1.0.15/protocol0/domain/lom/note/Note.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.833907 protocol0-1.0.15/protocol0/domain/lom/sample/__init__.py
+-rw-r--r--   0        0        0     3450 2023-06-04 21:57:43.692163 protocol0-1.0.15/protocol0/domain/lom/sample/SampleCategory.py
+-rw-r--r--   0        0        0     1235 2023-06-04 10:45:57.832742 protocol0-1.0.15/protocol0/domain/lom/sample/SampleCategoryEnum.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.859520 protocol0-1.0.15/protocol0/domain/lom/scene/__init__.py
+-rw-r--r--   0        0        0     1199 2023-06-04 10:45:57.834937 protocol0-1.0.15/protocol0/domain/lom/scene/LoopingSceneToggler.py
+-rw-r--r--   0        0        0      362 2023-06-04 21:57:43.524158 protocol0-1.0.15/protocol0/domain/lom/scene/NextSceneStartedEvent.py
+-rw-r--r--   0        0        0       51 2023-06-04 10:45:57.838723 protocol0-1.0.15/protocol0/domain/lom/scene/PlayingSceneChangedEvent.py
+-rw-r--r--   0        0        0     2895 2023-06-04 21:57:43.953222 protocol0-1.0.15/protocol0/domain/lom/scene/PlayingSceneFacade.py
+-rw-r--r--   0        0        0     8509 2023-06-04 21:57:44.308755 protocol0-1.0.15/protocol0/domain/lom/scene/Scene.py
+-rw-r--r--   0        0        0      887 2023-06-04 10:45:57.841452 protocol0-1.0.15/protocol0/domain/lom/scene/SceneAppearance.py
+-rw-r--r--   0        0        0     3472 2023-06-04 10:45:57.843216 protocol0-1.0.15/protocol0/domain/lom/scene/SceneClips.py
+-rw-r--r--   0        0        0      735 2023-06-04 10:45:57.844263 protocol0-1.0.15/protocol0/domain/lom/scene/SceneCropScroller.py
+-rw-r--r--   0        0        0      204 2023-06-04 21:57:43.597159 protocol0-1.0.15/protocol0/domain/lom/scene/SceneFiredEvent.py
+-rw-r--r--   0        0        0      263 2023-06-04 10:45:57.846254 protocol0-1.0.15/protocol0/domain/lom/scene/SceneLastBarPassedEvent.py
+-rw-r--r--   0        0        0     2376 2023-06-04 10:45:57.847262 protocol0-1.0.15/protocol0/domain/lom/scene/SceneLength.py
+-rw-r--r--   0        0        0     3560 2023-06-04 10:45:57.848324 protocol0-1.0.15/protocol0/domain/lom/scene/SceneName.py
+-rw-r--r--   0        0        0     5743 2023-06-04 10:45:57.849839 protocol0-1.0.15/protocol0/domain/lom/scene/ScenePlaybackService.py
+-rw-r--r--   0        0        0     1973 2023-06-04 21:57:43.914220 protocol0-1.0.15/protocol0/domain/lom/scene/ScenePlayingState.py
+-rw-r--r--   0        0        0       53 2023-06-04 10:45:57.851893 protocol0-1.0.15/protocol0/domain/lom/scene/ScenePositionScrolledEvent.py
+-rw-r--r--   0        0        0     1773 2023-06-04 21:53:36.526420 protocol0-1.0.15/protocol0/domain/lom/scene/ScenePositionScroller.py
+-rw-r--r--   0        0        0     6158 2023-06-04 21:57:44.061219 protocol0-1.0.15/protocol0/domain/lom/scene/SceneService.py
+-rw-r--r--   0        0        0       44 2023-06-04 10:45:57.858472 protocol0-1.0.15/protocol0/domain/lom/scene/ScenesMappedEvent.py
+-rw-r--r--   0        0        0     3355 2023-06-04 10:45:57.855477 protocol0-1.0.15/protocol0/domain/lom/scene/SceneWindow.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.866109 protocol0-1.0.15/protocol0/domain/lom/set/__init__.py
+-rw-r--r--   0        0        0     4599 2023-06-04 21:57:43.977223 protocol0-1.0.15/protocol0/domain/lom/set/AbletonSet.py
+-rw-r--r--   0        0        0      270 2023-06-04 10:45:57.861519 protocol0-1.0.15/protocol0/domain/lom/set/AbletonSetChangedEvent.py
+-rw-r--r--   0        0        0      420 2023-06-04 10:45:57.863528 protocol0-1.0.15/protocol0/domain/lom/set/MixingService.py
+-rw-r--r--   0        0        0     6197 2023-06-04 10:45:57.866109 protocol0-1.0.15/protocol0/domain/lom/set/SessionToArrangementService.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.872912 protocol0-1.0.15/protocol0/domain/lom/song/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.887048 protocol0-1.0.15/protocol0/domain/lom/song/components/__init__.py
+-rw-r--r--   0        0        0     2528 2023-06-04 10:45:57.874402 protocol0-1.0.15/protocol0/domain/lom/song/components/ClipComponent.py
+-rw-r--r--   0        0        0     2480 2023-06-04 10:45:57.875793 protocol0-1.0.15/protocol0/domain/lom/song/components/DeviceComponent.py
+-rw-r--r--   0        0        0     5230 2023-06-04 10:45:57.877999 protocol0-1.0.15/protocol0/domain/lom/song/components/PlaybackComponent.py
+-rw-r--r--   0        0        0     1177 2023-06-04 10:45:57.879009 protocol0-1.0.15/protocol0/domain/lom/song/components/QuantizationComponent.py
+-rw-r--r--   0        0        0     2950 2023-06-04 10:45:57.880010 protocol0-1.0.15/protocol0/domain/lom/song/components/RecordingComponent.py
+-rw-r--r--   0        0        0     2288 2023-06-04 10:45:57.881044 protocol0-1.0.15/protocol0/domain/lom/song/components/SceneComponent.py
+-rw-r--r--   0        0        0     2543 2023-06-04 10:45:57.882006 protocol0-1.0.15/protocol0/domain/lom/song/components/SceneCrudComponent.py
+-rw-r--r--   0        0        0     1179 2023-06-04 10:45:57.883047 protocol0-1.0.15/protocol0/domain/lom/song/components/TempoComponent.py
+-rw-r--r--   0        0        0     4790 2023-06-04 10:45:57.884024 protocol0-1.0.15/protocol0/domain/lom/song/components/TrackComponent.py
+-rw-r--r--   0        0        0     2028 2023-06-04 10:45:57.886036 protocol0-1.0.15/protocol0/domain/lom/song/components/TrackCrudComponent.py
+-rw-r--r--   0        0        0       47 2023-06-04 10:45:57.868938 protocol0-1.0.15/protocol0/domain/lom/song/SongInitializedEvent.py
+-rw-r--r--   0        0        0     2090 2023-06-04 10:45:57.867906 protocol0-1.0.15/protocol0/domain/lom/song/SongInitService.py
+-rw-r--r--   0        0        0       43 2023-06-04 10:45:57.869923 protocol0-1.0.15/protocol0/domain/lom/song/SongStartedEvent.py
+-rw-r--r--   0        0        0       43 2023-06-04 10:45:57.871952 protocol0-1.0.15/protocol0/domain/lom/song/SongStoppedEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.899961 protocol0-1.0.15/protocol0/domain/lom/track/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.906980 protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/__init__.py
+-rw-r--r--   0        0        0     1507 2023-06-04 21:57:43.815218 protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/AbstrackTrackArmState.py
+-rw-r--r--   0        0        0     6108 2023-06-04 10:45:57.902939 protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/AbstractTrack.py
+-rw-r--r--   0        0        0     2203 2023-06-04 10:45:57.904964 protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/AbstractTrackAppearance.py
+-rw-r--r--   0        0        0       56 2023-06-04 10:45:57.905965 protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/AbstractTrackNameUpdatedEvent.py
+-rw-r--r--   0        0        0      179 2023-06-04 10:45:57.906980 protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/AbstractTrackSelectedEvent.py
+-rw-r--r--   0        0        0      135 2023-06-04 10:45:57.888738 protocol0-1.0.15/protocol0/domain/lom/track/CurrentMonitoringStateEnum.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.915229 protocol0-1.0.15/protocol0/domain/lom/track/group_track/__init__.py
+-rw-r--r--   0        0        0     3797 2023-06-04 10:45:57.909040 protocol0-1.0.15/protocol0/domain/lom/track/group_track/AbstractGroupTrack.py
+-rw-r--r--   0        0        0      385 2023-06-04 10:45:57.910200 protocol0-1.0.15/protocol0/domain/lom/track/group_track/DrumsTrack.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.929035 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/__init__.py
+-rw-r--r--   0        0        0      271 2023-06-04 10:45:57.919261 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtArmedEvent.py
+-rw-r--r--   0        0        0     2167 2023-06-04 21:57:43.899221 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtArmState.py
+-rw-r--r--   0        0        0     4340 2023-06-04 10:45:57.925796 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExternalSynthTrack.py
+-rw-r--r--   0        0        0     2541 2023-06-04 21:57:43.963223 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtMatchingTrack.py
+-rw-r--r--   0        0        0     2998 2023-06-04 21:57:44.006221 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py
+-rw-r--r--   0        0        0     1952 2023-06-04 10:45:57.922784 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtMonitoringState.py
+-rw-r--r--   0        0        0     2115 2023-06-04 10:45:57.923790 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtSoloState.py
+-rw-r--r--   0        0        0      662 2023-06-04 10:45:57.926791 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py
+-rw-r--r--   0        0        0      887 2023-06-04 21:57:43.881220 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py
+-rw-r--r--   0        0        0      746 2023-06-04 21:57:43.881220 protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.940091 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/__init__.py
+-rw-r--r--   0        0        0     2002 2023-06-04 10:45:57.931555 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py
+-rw-r--r--   0        0        0     3644 2023-06-04 10:45:57.932599 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py
+-rw-r--r--   0        0        0      645 2023-06-04 10:45:57.934573 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py
+-rw-r--r--   0        0        0     2055 2023-06-04 10:45:57.935619 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackInterface.py
+-rw-r--r--   0        0        0     2334 2023-06-04 21:57:44.076223 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackRouter.py
+-rw-r--r--   0        0        0     7279 2023-06-04 10:45:57.938582 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackService.py
+-rw-r--r--   0        0        0      956 2023-06-04 10:45:57.939645 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py
+-rw-r--r--   0        0        0     2159 2023-06-04 10:45:57.941095 protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/utils.py
+-rw-r--r--   0        0        0      982 2023-06-04 21:57:43.959223 protocol0-1.0.15/protocol0/domain/lom/track/group_track/NormalGroupMatchingTrack.py
+-rw-r--r--   0        0        0     1548 2023-06-04 21:57:44.027227 protocol0-1.0.15/protocol0/domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py
+-rw-r--r--   0        0        0     3760 2023-06-04 21:57:44.193221 protocol0-1.0.15/protocol0/domain/lom/track/group_track/NormalGroupTrack.py
+-rw-r--r--   0        0        0      155 2023-06-04 10:45:57.915229 protocol0-1.0.15/protocol0/domain/lom/track/group_track/VocalsTrack.py
+-rw-r--r--   0        0        0      205 2023-06-04 10:45:57.889495 protocol0-1.0.15/protocol0/domain/lom/track/P0TrackInterface.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.952086 protocol0-1.0.15/protocol0/domain/lom/track/routing/__init__.py
+-rw-r--r--   0        0        0      237 2023-06-04 10:45:57.943098 protocol0-1.0.15/protocol0/domain/lom/track/routing/InputRoutingChannelEnum.py
+-rw-r--r--   0        0        0      251 2023-06-04 10:45:57.944404 protocol0-1.0.15/protocol0/domain/lom/track/routing/InputRoutingTypeEnum.py
+-rw-r--r--   0        0        0      251 2023-06-04 10:45:57.946061 protocol0-1.0.15/protocol0/domain/lom/track/routing/OutputRoutingTypeEnum.py
+-rw-r--r--   0        0        0     1786 2023-06-04 10:45:57.947103 protocol0-1.0.15/protocol0/domain/lom/track/routing/RoutingDisplayNameDescriptor.py
+-rw-r--r--   0        0        0     3576 2023-06-04 10:45:57.948137 protocol0-1.0.15/protocol0/domain/lom/track/routing/RoutingTrackDescriptor.py
+-rw-r--r--   0        0        0      779 2023-06-04 10:45:57.949064 protocol0-1.0.15/protocol0/domain/lom/track/routing/TrackInputRouting.py
+-rw-r--r--   0        0        0      595 2023-06-04 10:45:57.950090 protocol0-1.0.15/protocol0/domain/lom/track/routing/TrackOutputRouting.py
+-rw-r--r--   0        0        0      441 2023-06-04 10:45:57.951090 protocol0-1.0.15/protocol0/domain/lom/track/routing/TrackRoutingInterface.py
+-rw-r--r--   0        0        0       52 2023-06-04 10:45:57.891724 protocol0-1.0.15/protocol0/domain/lom/track/SelectedTrackChangedEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.972856 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.976822 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.978834 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/master/__init__.py
+-rw-r--r--   0        0        0     1999 2023-06-04 21:57:44.122221 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/master/MasterTrack.py
+-rw-r--r--   0        0        0     4947 2023-06-04 10:45:57.973857 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/SimpleAudioTrack.py
+-rw-r--r--   0        0        0      626 2023-06-04 21:57:44.046226 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/SimpleReturnTrack.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.983751 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/special/__init__.py
+-rw-r--r--   0        0        0     1225 2023-06-04 21:57:44.142222 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/special/ReferenceTrack.py
+-rw-r--r--   0        0        0      397 2023-06-04 10:45:57.983751 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/special/ResamplingTrack.py
+-rw-r--r--   0        0        0     2912 2023-06-04 10:45:57.953359 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/AudioToMidiClipMapping.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.986654 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/midi/__init__.py
+-rw-r--r--   0        0        0     1566 2023-06-04 10:45:57.985595 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/midi/SimpleMidiTrack.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.988689 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/midi/special/__init__.py
+-rw-r--r--   0        0        0     2686 2023-06-04 21:57:44.193221 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/midi/special/UsamoTrack.py
+-rw-r--r--   0        0        0     2645 2023-06-04 21:57:44.156217 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleMatchingTrack.py
+-rw-r--r--   0        0        0     1583 2023-06-04 21:57:44.255754 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleMatchingTrackCreator.py
+-rw-r--r--   0        0        0    16256 2023-06-04 10:45:57.957888 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrack.py
+-rw-r--r--   0        0        0      174 2023-06-04 10:45:57.960123 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackArmedEvent.py
+-rw-r--r--   0        0        0     1375 2023-06-04 10:45:57.958888 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackArmState.py
+-rw-r--r--   0        0        0     1359 2023-06-04 21:57:44.118219 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackClipColorManager.py
+-rw-r--r--   0        0        0     1068 2023-06-04 21:57:44.119220 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackClips.py
+-rw-r--r--   0        0        0     4736 2023-06-04 21:57:44.503759 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackClipSlots.py
+-rw-r--r--   0        0        0      279 2023-06-04 10:45:57.965856 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackCreatedEvent.py
+-rw-r--r--   0        0        0      279 2023-06-04 10:45:57.966854 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackDeletedEvent.py
+-rw-r--r--   0        0        0      247 2023-06-04 10:45:57.967854 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackFlattenedEvent.py
+-rw-r--r--   0        0        0     1219 2023-06-04 10:45:57.968854 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackMonitoringState.py
+-rw-r--r--   0        0        0       54 2023-06-04 10:45:57.969856 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackSaveStartedEvent.py
+-rw-r--r--   0        0        0      898 2023-06-04 21:57:44.128223 protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackService.py
+-rw-r--r--   0        0        0       42 2023-06-04 10:45:57.892742 protocol0-1.0.15/protocol0/domain/lom/track/TrackAddedEvent.py
+-rw-r--r--   0        0        0     6108 2023-06-04 21:57:44.443757 protocol0-1.0.15/protocol0/domain/lom/track/TrackAutomationService.py
+-rw-r--r--   0        0        0      166 2023-06-04 10:45:57.894600 protocol0-1.0.15/protocol0/domain/lom/track/TrackColorEnum.py
+-rw-r--r--   0        0        0      286 2023-06-04 10:45:57.895710 protocol0-1.0.15/protocol0/domain/lom/track/TrackDisconnectedEvent.py
+-rw-r--r--   0        0        0     4775 2023-06-04 21:57:44.448757 protocol0-1.0.15/protocol0/domain/lom/track/TrackFactory.py
+-rw-r--r--   0        0        0     8797 2023-06-04 21:57:44.898820 protocol0-1.0.15/protocol0/domain/lom/track/TrackMapperService.py
+-rw-r--r--   0        0        0     1054 2023-06-04 10:45:57.898935 protocol0-1.0.15/protocol0/domain/lom/track/TrackService.py
+-rw-r--r--   0        0        0       44 2023-06-04 10:45:57.899961 protocol0-1.0.15/protocol0/domain/lom/track/TracksMappedEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.994476 protocol0-1.0.15/protocol0/domain/lom/validation/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.001537 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/__init__.py
+-rw-r--r--   0        0        0      385 2023-06-04 10:45:57.996814 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/AbstractGroupTrackValidator.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.006595 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/external_synth_track/__init__.py
+-rw-r--r--   0        0        0     2097 2023-06-04 10:45:58.002971 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py
+-rw-r--r--   0        0        0     1735 2023-06-04 10:45:58.004966 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py
+-rw-r--r--   0        0        0     2102 2023-06-04 21:57:44.250755 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py
+-rw-r--r--   0        0        0      950 2023-06-04 10:45:57.998089 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/SceneValidator.py
+-rw-r--r--   0        0        0      938 2023-06-04 10:45:57.999904 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/SimpleAudioTrackValidator.py
+-rw-r--r--   0        0        0      413 2023-06-04 10:45:58.000951 protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/SimpleTrackValidator.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.015692 protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/__init__.py
+-rw-r--r--   0        0        0     1053 2023-06-04 21:57:44.228755 protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/AggregateValidator.py
+-rw-r--r--   0        0        0     1106 2023-06-04 10:45:58.010299 protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/CallbackValidator.py
+-rw-r--r--   0        0        0     1570 2023-06-04 10:45:58.012313 protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/DeviceParameterValidator.py
+-rw-r--r--   0        0        0     1912 2023-06-04 10:45:58.013680 protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/PropertyValueValidator.py
+-rw-r--r--   0        0        0     1355 2023-06-04 10:45:58.014690 protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py
+-rw-r--r--   0        0        0     2173 2023-06-04 10:45:57.991020 protocol0-1.0.15/protocol0/domain/lom/validation/ValidatorFactory.py
+-rw-r--r--   0        0        0      559 2023-06-04 10:45:57.992298 protocol0-1.0.15/protocol0/domain/lom/validation/ValidatorInterface.py
+-rw-r--r--   0        0        0     1897 2023-06-04 10:45:57.994476 protocol0-1.0.15/protocol0/domain/lom/validation/ValidatorService.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.027208 protocol0-1.0.15/protocol0/domain/shared/__init__.py
+-rw-r--r--   0        0        0     3720 2023-06-04 10:45:58.016585 protocol0-1.0.15/protocol0/domain/shared/ApplicationView.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.031631 protocol0-1.0.15/protocol0/domain/shared/backend/__init__.py
+-rw-r--r--   0        0        0     1410 2023-06-04 16:32:04.016831 protocol0-1.0.15/protocol0/domain/shared/backend/Backend.py
+-rw-r--r--   0        0        0      190 2023-06-04 10:45:58.029503 protocol0-1.0.15/protocol0/domain/shared/backend/BackendEvent.py
+-rw-r--r--   0        0        0      103 2023-06-04 10:45:58.030619 protocol0-1.0.15/protocol0/domain/shared/backend/NotificationColorEnum.py
+-rw-r--r--   0        0        0    24899 2023-06-04 21:57:45.472003 protocol0-1.0.15/protocol0/domain/shared/backend/p0_backend_client/api/default_api.py
+-rw-r--r--   0        0        0      644 2023-06-04 10:45:58.018432 protocol0-1.0.15/protocol0/domain/shared/BrowserServiceInterface.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.035738 protocol0-1.0.15/protocol0/domain/shared/errors/__init__.py
+-rw-r--r--   0        0        0      605 2023-06-04 10:45:58.038272 protocol0-1.0.15/protocol0/domain/shared/errors/error_handler.py
+-rw-r--r--   0        0        0      178 2023-06-04 10:45:58.033562 protocol0-1.0.15/protocol0/domain/shared/errors/ErrorRaisedEvent.py
+-rw-r--r--   0        0        0       47 2023-06-04 10:45:58.034726 protocol0-1.0.15/protocol0/domain/shared/errors/Protocol0Error.py
+-rw-r--r--   0        0        0      359 2023-06-04 10:45:58.035738 protocol0-1.0.15/protocol0/domain/shared/errors/Protocol0Warning.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.041860 protocol0-1.0.15/protocol0/domain/shared/event/__init__.py
+-rw-r--r--   0        0        0     4775 2023-06-04 10:45:58.040274 protocol0-1.0.15/protocol0/domain/shared/event/DomainEventBus.py
+-rw-r--r--   0        0        0      200 2023-06-04 10:45:58.040853 protocol0-1.0.15/protocol0/domain/shared/event/HasEmitter.py
+-rw-r--r--   0        0        0      118 2023-06-04 10:45:58.020445 protocol0-1.0.15/protocol0/domain/shared/InterfaceClicksServiceInterface.py
+-rw-r--r--   0        0        0      569 2023-06-04 21:57:44.401757 protocol0-1.0.15/protocol0/domain/shared/LiveObject.py
+-rw-r--r--   0        0        0     1966 2023-06-04 10:45:58.022784 protocol0-1.0.15/protocol0/domain/shared/LiveObjectMapping.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.057489 protocol0-1.0.15/protocol0/domain/shared/scheduler/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-04 10:45:58.043249 protocol0-1.0.15/protocol0/domain/shared/scheduler/BarChangedEvent.py
+-rw-r--r--   0        0        0       41 2023-06-04 10:45:58.045279 protocol0-1.0.15/protocol0/domain/shared/scheduler/BarEndingEvent.py
+-rw-r--r--   0        0        0      309 2023-06-04 10:45:58.046880 protocol0-1.0.15/protocol0/domain/shared/scheduler/BeatSchedulerInterface.py
+-rw-r--r--   0        0        0       46 2023-06-04 10:45:58.048660 protocol0-1.0.15/protocol0/domain/shared/scheduler/Last16thPassedEvent.py
+-rw-r--r--   0        0        0       46 2023-06-04 10:45:58.049670 protocol0-1.0.15/protocol0/domain/shared/scheduler/Last32thPassedEvent.py
+-rw-r--r--   0        0        0       45 2023-06-04 10:45:58.050669 protocol0-1.0.15/protocol0/domain/shared/scheduler/Last8thPassedEvent.py
+-rw-r--r--   0        0        0       46 2023-06-04 10:45:58.051880 protocol0-1.0.15/protocol0/domain/shared/scheduler/LastBeatPassedEvent.py
+-rw-r--r--   0        0        0     2574 2023-06-04 21:57:44.421755 protocol0-1.0.15/protocol0/domain/shared/scheduler/Scheduler.py
+-rw-r--r--   0        0        0       47 2023-06-04 10:45:58.053931 protocol0-1.0.15/protocol0/domain/shared/scheduler/ThirdBeatPassedEvent.py
+-rw-r--r--   0        0        0      130 2023-06-04 10:45:58.055529 protocol0-1.0.15/protocol0/domain/shared/scheduler/TickSchedulerEventInterface.py
+-rw-r--r--   0        0        0      565 2023-06-04 10:45:58.056527 protocol0-1.0.15/protocol0/domain/shared/scheduler/TickSchedulerInterface.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.058511 protocol0-1.0.15/protocol0/domain/shared/script/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-04 10:45:58.023784 protocol0-1.0.15/protocol0/domain/shared/SessionServiceInterface.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.061074 protocol0-1.0.15/protocol0/domain/shared/ui/__init__.py
+-rw-r--r--   0        0        0      128 2023-06-04 10:45:58.061074 protocol0-1.0.15/protocol0/domain/shared/ui/ColorEnum.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.062827 protocol0-1.0.15/protocol0/domain/shared/utils/__init__.py
+-rw-r--r--   0        0        0      974 2023-06-04 10:45:58.064086 protocol0-1.0.15/protocol0/domain/shared/utils/concurrency.py
+-rw-r--r--   0        0        0      950 2023-06-04 21:51:56.115129 protocol0-1.0.15/protocol0/domain/shared/utils/debug.py
+-rw-r--r--   0        0        0     1607 2023-06-04 10:45:58.066096 protocol0-1.0.15/protocol0/domain/shared/utils/forward_to.py
+-rw-r--r--   0        0        0     3219 2023-06-04 21:57:44.582755 protocol0-1.0.15/protocol0/domain/shared/utils/func.py
+-rw-r--r--   0        0        0      270 2023-06-04 10:45:58.069412 protocol0-1.0.15/protocol0/domain/shared/utils/list.py
+-rw-r--r--   0        0        0      294 2023-06-04 21:51:18.909132 protocol0-1.0.15/protocol0/domain/shared/utils/string.py
+-rw-r--r--   0        0        0     4821 2023-06-04 21:57:44.730291 protocol0-1.0.15/protocol0/domain/shared/utils/timing.py
+-rw-r--r--   0        0        0     3500 2023-06-04 21:52:25.322303 protocol0-1.0.15/protocol0/domain/shared/utils/utils.py
+-rw-r--r--   0        0        0     2247 2023-06-04 10:45:58.024783 protocol0-1.0.15/protocol0/domain/shared/ValueScroller.py
+-rw-r--r--   0        0        0     1003 2023-06-04 10:45:58.025785 protocol0-1.0.15/protocol0/domain/shared/ValueToggler.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.082256 protocol0-1.0.15/protocol0/domain/track_recorder/__init__.py
+-rw-r--r--   0        0        0      687 2023-06-04 10:45:58.075832 protocol0-1.0.15/protocol0/domain/track_recorder/AbstractRecorderFactory.py
+-rw-r--r--   0        0        0     3284 2023-06-04 21:57:44.562756 protocol0-1.0.15/protocol0/domain/track_recorder/BaseRecorder.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.086834 protocol0-1.0.15/protocol0/domain/track_recorder/config/__init__.py
+-rw-r--r--   0        0        0     1809 2023-06-04 10:45:58.084242 protocol0-1.0.15/protocol0/domain/track_recorder/config/RecordConfig.py
+-rw-r--r--   0        0        0     1180 2023-06-04 21:57:44.542756 protocol0-1.0.15/protocol0/domain/track_recorder/config/RecordProcessors.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.093102 protocol0-1.0.15/protocol0/domain/track_recorder/count_in/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-04 10:45:58.089216 protocol0-1.0.15/protocol0/domain/track_recorder/count_in/CountInInterface.py
+-rw-r--r--   0        0        0     1663 2023-06-04 10:45:58.091089 protocol0-1.0.15/protocol0/domain/track_recorder/count_in/CountInOneBar.py
+-rw-r--r--   0        0        0      645 2023-06-04 10:45:58.092101 protocol0-1.0.15/protocol0/domain/track_recorder/count_in/CountInShort.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.098582 protocol0-1.0.15/protocol0/domain/track_recorder/event/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-04 10:45:58.095096 protocol0-1.0.15/protocol0/domain/track_recorder/event/RecordCancelledEvent.py
+-rw-r--r--   0        0        0       43 2023-06-04 21:57:44.449756 protocol0-1.0.15/protocol0/domain/track_recorder/event/RecordEndedEvent.py
+-rw-r--r--   0        0        0      265 2023-06-04 10:45:58.098582 protocol0-1.0.15/protocol0/domain/track_recorder/event/RecordStartedEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.108560 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-04 10:45:58.100899 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/AudioClipSilentEvent.py
+-rw-r--r--   0        0        0      265 2023-06-04 10:45:58.101897 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/ExtAudioRecordingEndedEvent.py
+-rw-r--r--   0        0        0      267 2023-06-04 10:45:58.105102 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/ExtAudioRecordingStartedEvent.py
+-rw-r--r--   0        0        0     3045 2023-06-04 21:57:44.637756 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/OnRecordEndClipTail.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.114071 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/__init__.py
+-rw-r--r--   0        0        0     1958 2023-06-04 10:45:58.109961 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/PostRecordAudio.py
+-rw-r--r--   0        0        0      991 2023-06-04 21:57:44.515753 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py
+-rw-r--r--   0        0        0     1012 2023-06-04 21:57:44.502756 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/PreRecordAudio.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.117785 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/__init__.py
+-rw-r--r--   0        0        0     2580 2023-06-04 21:57:44.651754 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py
+-rw-r--r--   0        0        0     2184 2023-06-04 21:57:44.595760 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.123358 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_midi/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-04 10:45:58.121310 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_midi/PostRecordMidi.py
+-rw-r--r--   0        0        0      466 2023-06-04 21:57:44.481758 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_midi/PreRecordMidi.py
+-rw-r--r--   0        0        0     4780 2023-06-04 10:45:58.107495 protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.128660 protocol0-1.0.15/protocol0/domain/track_recorder/recording_bar_length/__init__.py
+-rw-r--r--   0        0        0      565 2023-06-04 10:45:58.124470 protocol0-1.0.15/protocol0/domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py
+-rw-r--r--   0        0        0      890 2023-06-04 10:45:58.126481 protocol0-1.0.15/protocol0/domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py
+-rw-r--r--   0        0        0       65 2023-06-04 10:45:58.128660 protocol0-1.0.15/protocol0/domain/track_recorder/recording_bar_length/SelectedRecordingBarLengthUpdatedEvent.py
+-rw-r--r--   0        0        0      670 2023-06-04 10:45:58.079235 protocol0-1.0.15/protocol0/domain/track_recorder/RecordProcessorInterface.py
+-rw-r--r--   0        0        0     7834 2023-06-04 21:57:45.033991 protocol0-1.0.15/protocol0/domain/track_recorder/RecordService.py
+-rw-r--r--   0        0        0      897 2023-06-04 10:45:58.082256 protocol0-1.0.15/protocol0/domain/track_recorder/RecordTypeEnum.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.132602 protocol0-1.0.15/protocol0/domain/track_recorder/simple/__init__.py
+-rw-r--r--   0        0        0      703 2023-06-04 10:45:58.130592 protocol0-1.0.15/protocol0/domain/track_recorder/simple/PostRecordSimple.py
+-rw-r--r--   0        0        0     2241 2023-06-04 21:57:44.743291 protocol0-1.0.15/protocol0/domain/track_recorder/simple/RecorderSimpleFactory.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.133797 protocol0-1.0.15/protocol0/infra/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.141735 protocol0-1.0.15/protocol0/infra/interface/__init__.py
+-rw-r--r--   0        0        0     5528 2023-06-04 21:52:14.241022 protocol0-1.0.15/protocol0/infra/interface/BrowserLoaderService.py
+-rw-r--r--   0        0        0     2790 2023-06-04 10:45:58.138487 protocol0-1.0.15/protocol0/infra/interface/BrowserService.py
+-rw-r--r--   0        0        0      427 2023-06-04 10:45:58.139987 protocol0-1.0.15/protocol0/infra/interface/InterfaceClicksService.py
+-rw-r--r--   0        0        0      262 2023-06-04 10:45:58.140959 protocol0-1.0.15/protocol0/infra/interface/PixelEnum.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.145747 protocol0-1.0.15/protocol0/infra/interface/session/__init__.py
+-rw-r--r--   0        0        0     2470 2023-06-04 21:55:06.318647 protocol0-1.0.15/protocol0/infra/interface/session/SessionService.py
+-rw-r--r--   0        0        0      226 2023-06-04 10:45:58.144783 protocol0-1.0.15/protocol0/infra/interface/session/SessionUpdatedEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.147763 protocol0-1.0.15/protocol0/infra/logging/__init__.py
+-rw-r--r--   0        0        0     2075 2023-06-04 21:50:51.471107 protocol0-1.0.15/protocol0/infra/logging/LoggerService.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.153445 protocol0-1.0.15/protocol0/infra/midi/__init__.py
+-rw-r--r--   0        0        0      177 2023-06-04 10:45:58.148782 protocol0-1.0.15/protocol0/infra/midi/MidiBytesReceivedEvent.py
+-rw-r--r--   0        0        0      173 2023-06-04 10:45:58.149808 protocol0-1.0.15/protocol0/infra/midi/MidiBytesSentEvent.py
+-rw-r--r--   0        0        0     3279 2023-06-04 10:45:58.152441 protocol0-1.0.15/protocol0/infra/midi/MidiService.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.160342 protocol0-1.0.15/protocol0/infra/persistence/__init__.py
+-rw-r--r--   0        0        0      254 2023-06-04 10:45:58.155275 protocol0-1.0.15/protocol0/infra/persistence/SongDataEnum.py
+-rw-r--r--   0        0        0     3038 2023-06-04 21:57:44.850822 protocol0-1.0.15/protocol0/infra/persistence/SongDataService.py
+-rw-r--r--   0        0        0     1229 2023-06-04 10:45:58.159336 protocol0-1.0.15/protocol0/infra/persistence/TrackData.py
+-rw-r--r--   0        0        0      131 2023-06-04 10:45:58.160342 protocol0-1.0.15/protocol0/infra/persistence/TrackDataEnum.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.169857 protocol0-1.0.15/protocol0/infra/scheduler/__init__.py
+-rw-r--r--   0        0        0     5140 2023-06-04 10:45:58.163172 protocol0-1.0.15/protocol0/infra/scheduler/BeatScheduler.py
+-rw-r--r--   0        0        0      862 2023-06-04 21:57:44.689760 protocol0-1.0.15/protocol0/infra/scheduler/BeatSchedulerEvent.py
+-rw-r--r--   0        0        0     3806 2023-06-04 10:45:58.166164 protocol0-1.0.15/protocol0/infra/scheduler/BeatTime.py
+-rw-r--r--   0        0        0     2998 2023-06-04 10:45:58.167817 protocol0-1.0.15/protocol0/infra/scheduler/TickScheduler.py
+-rw-r--r--   0        0        0     1031 2023-06-04 10:45:58.168904 protocol0-1.0.15/protocol0/infra/scheduler/TickSchedulerEvent.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.177847 protocol0-1.0.15/protocol0/shared/__init__.py
+-rw-r--r--   0        0        0      813 2023-06-04 10:45:58.171851 protocol0-1.0.15/protocol0/shared/AbstractEnum.py
+-rw-r--r--   0        0        0      939 2023-06-04 21:57:44.790829 protocol0-1.0.15/protocol0/shared/Config.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.185840 protocol0-1.0.15/protocol0/shared/logging/__init__.py
+-rw-r--r--   0        0        0     1917 2023-06-04 10:45:58.182315 protocol0-1.0.15/protocol0/shared/logging/Logger.py
+-rw-r--r--   0        0        0      271 2023-06-04 10:45:58.183812 protocol0-1.0.15/protocol0/shared/logging/LoggerServiceInterface.py
+-rw-r--r--   0        0        0      154 2023-06-04 10:45:58.180268 protocol0-1.0.15/protocol0/shared/logging/LogLevelEnum.py
+-rw-r--r--   0        0        0      724 2023-06-04 10:45:58.184859 protocol0-1.0.15/protocol0/shared/logging/StatusBar.py
+-rw-r--r--   0        0        0     1050 2023-06-04 21:57:44.755290 protocol0-1.0.15/protocol0/shared/module.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.192173 protocol0-1.0.15/protocol0/shared/observer/__init__.py
+-rw-r--r--   0        0        0      702 2023-06-04 10:45:58.190170 protocol0-1.0.15/protocol0/shared/observer/Observable.py
+-rw-r--r--   0        0        0      259 2023-06-04 10:45:58.191217 protocol0-1.0.15/protocol0/shared/observer/Observer.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.251429 protocol0-1.0.15/protocol0/shared/sequence/__init__.py
+-rw-r--r--   0        0        0      708 2023-06-04 10:45:58.202610 protocol0-1.0.15/protocol0/shared/sequence/HasSequenceState.py
+-rw-r--r--   0        0        0     2073 2023-06-04 10:45:58.208602 protocol0-1.0.15/protocol0/shared/sequence/ParallelSequence.py
+-rw-r--r--   0        0        0    12095 2023-06-04 21:57:45.294944 protocol0-1.0.15/protocol0/shared/sequence/Sequence.py
+-rw-r--r--   0        0        0     1666 2023-06-04 10:45:58.226711 protocol0-1.0.15/protocol0/shared/sequence/SequenceState.py
+-rw-r--r--   0        0        0     2859 2023-06-04 10:45:58.230723 protocol0-1.0.15/protocol0/shared/sequence/SequenceStep.py
+-rw-r--r--   0        0        0      871 2023-06-04 10:45:58.239422 protocol0-1.0.15/protocol0/shared/sequence/SequenceTransition.py
+-rw-r--r--   0        0        0     1801 2023-06-04 10:45:58.247419 protocol0-1.0.15/protocol0/shared/sequence/TimeoutLimit.py
+-rw-r--r--   0        0        0    14092 2023-06-04 21:57:45.406616 protocol0-1.0.15/protocol0/shared/Song.py
+-rw-r--r--   0        0        0      127 2023-06-04 10:45:58.257696 protocol0-1.0.15/protocol0/shared/types.py
+-rw-r--r--   0        0        0      594 2023-06-04 21:57:44.780822 protocol0-1.0.15/protocol0/shared/UndoFacade.py
+-rw-r--r--   0        0        0      230 2023-06-04 10:45:58.267194 protocol0-1.0.15/protocol0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.270276 protocol0-1.0.15/protocol0/tests/application/__init__.py
+-rw-r--r--   0        0        0     2810 2023-06-04 10:45:58.277181 protocol0-1.0.15/protocol0/tests/application/test_multi_encoder.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.279877 protocol0-1.0.15/protocol0/tests/domain/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.288235 protocol0-1.0.15/protocol0/tests/domain/clip/__init__.py
+-rw-r--r--   0        0        0      853 2023-06-04 10:45:58.291234 protocol0-1.0.15/protocol0/tests/domain/clip/test_clip_playing_position.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.293231 protocol0-1.0.15/protocol0/tests/domain/fixtures/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-04 10:45:58.295525 protocol0-1.0.15/protocol0/tests/domain/fixtures/clip.py
+-rw-r--r--   0        0        0      447 2023-06-04 10:45:58.296527 protocol0-1.0.15/protocol0/tests/domain/fixtures/clip_slot.py
+-rw-r--r--   0        0        0       72 2023-06-04 10:45:58.298540 protocol0-1.0.15/protocol0/tests/domain/fixtures/clip_view.py
+-rw-r--r--   0        0        0      261 2023-06-04 10:45:58.300169 protocol0-1.0.15/protocol0/tests/domain/fixtures/container.py
+-rw-r--r--   0        0        0      665 2023-06-04 10:45:58.302297 protocol0-1.0.15/protocol0/tests/domain/fixtures/device.py
+-rw-r--r--   0        0        0      319 2023-06-04 10:45:58.303346 protocol0-1.0.15/protocol0/tests/domain/fixtures/device_parameter.py
+-rw-r--r--   0        0        0      872 2023-06-04 10:45:58.304365 protocol0-1.0.15/protocol0/tests/domain/fixtures/group_track.py
+-rw-r--r--   0        0        0     2676 2023-06-04 21:57:45.052993 protocol0-1.0.15/protocol0/tests/domain/fixtures/p0.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.103453 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:57.102452 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/_Framework/__init__.py
+-rw-r--r--   0        0        0       58 2023-06-04 16:24:23.933052 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/_Framework/ButtonElement.py
+-rw-r--r--   0        0        0       63 2023-06-04 16:21:55.229396 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/_Framework/CompoundElement.py
+-rw-r--r--   0        0        0      218 2023-06-04 21:57:44.820429 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/_Framework/ControlSurface.py
+-rw-r--r--   0        0        0       38 2023-06-04 10:45:57.100454 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/_Framework/InputControlElement.py
+-rw-r--r--   0        0        0       61 2023-06-04 16:24:33.643552 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/_Framework/SessionComponent.py
+-rw-r--r--   0        0        0      142 2023-06-04 21:57:44.814826 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/_Framework/SubjectSlot.py
+-rw-r--r--   0        0        0      342 2023-06-04 10:45:57.104982 protocol0-1.0.15/protocol0/tests/domain/fixtures/protocol0_stub/setup.py
+-rw-r--r--   0        0        0      264 2023-06-04 10:45:58.307497 protocol0-1.0.15/protocol0/tests/domain/fixtures/scene.py
+-rw-r--r--   0        0        0     3081 2023-06-04 21:57:45.087039 protocol0-1.0.15/protocol0/tests/domain/fixtures/simple_track.py
+-rw-r--r--   0        0        0     2731 2023-06-04 10:45:58.311536 protocol0-1.0.15/protocol0/tests/domain/fixtures/song.py
+-rw-r--r--   0        0        0      308 2023-06-04 10:45:58.312968 protocol0-1.0.15/protocol0/tests/domain/fixtures/song_view.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.313964 protocol0-1.0.15/protocol0/tests/domain/scene/__init__.py
+-rw-r--r--   0        0        0      587 2023-06-04 21:56:40.465637 protocol0-1.0.15/protocol0/tests/domain/scene/test_scene_clips.py
+-rw-r--r--   0        0        0     1248 2023-06-04 10:45:58.317666 protocol0-1.0.15/protocol0/tests/domain/scene/test_scene_length.py
+-rw-r--r--   0        0        0     1351 2023-06-04 10:45:58.320727 protocol0-1.0.15/protocol0/tests/domain/scene/test_scene_playing_position.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.321873 protocol0-1.0.15/protocol0/tests/domain/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.324109 protocol0-1.0.15/protocol0/tests/domain/shared/event/__init__.py
+-rw-r--r--   0        0        0     1207 2023-06-04 10:45:58.326131 protocol0-1.0.15/protocol0/tests/domain/shared/event/test_domain_event_bus.py
+-rw-r--r--   0        0        0      233 2023-06-04 10:45:58.328407 protocol0-1.0.15/protocol0/tests/domain/shared/test_decorators.py
+-rw-r--r--   0        0        0      943 2023-06-04 10:45:58.329468 protocol0-1.0.15/protocol0/tests/domain/shared/test_live_object_mapping.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.331417 protocol0-1.0.15/protocol0/tests/domain/shared/utils/__init__.py
+-rw-r--r--   0        0        0      607 2023-06-04 10:45:58.333484 protocol0-1.0.15/protocol0/tests/domain/shared/utils/test_func.py
+-rw-r--r--   0        0        0     1477 2023-06-04 10:45:58.334483 protocol0-1.0.15/protocol0/tests/domain/shared/utils/test_utils.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.336489 protocol0-1.0.15/protocol0/tests/domain/track/__init__.py
+-rw-r--r--   0        0        0      783 2023-06-04 21:57:44.910827 protocol0-1.0.15/protocol0/tests/domain/track/test_audio_to_midi_clip_mapping.py
+-rw-r--r--   0        0        0      906 2023-06-04 10:45:58.339673 protocol0-1.0.15/protocol0/tests/domain/track/test_instantiation.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.342672 protocol0-1.0.15/protocol0/tests/domain/validation/__init__.py
+-rw-r--r--   0        0        0     1379 2023-06-04 10:45:58.345219 protocol0-1.0.15/protocol0/tests/domain/validation/test_aggregate_validator.py
+-rw-r--r--   0        0        0     1031 2023-06-04 10:45:58.347067 protocol0-1.0.15/protocol0/tests/domain/validation/test_callback_validator.py
+-rw-r--r--   0        0        0     1086 2023-06-04 10:45:58.350417 protocol0-1.0.15/protocol0/tests/domain/validation/test_property_validator.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.351476 protocol0-1.0.15/protocol0/tests/infra/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.353740 protocol0-1.0.15/protocol0/tests/infra/listeners/__init__.py
+-rw-r--r--   0        0        0     1301 2023-06-04 10:45:58.355876 protocol0-1.0.15/protocol0/tests/infra/listeners/test_subject_slot.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.361461 protocol0-1.0.15/protocol0/tests/infra/scheduler/__init__.py
+-rw-r--r--   0        0        0      504 2023-06-04 10:45:58.358766 protocol0-1.0.15/protocol0/tests/infra/scheduler/TickSchedulerEventTest.py
+-rw-r--r--   0        0        0      765 2023-06-04 10:45:58.360463 protocol0-1.0.15/protocol0/tests/infra/scheduler/TickSchedulerTest.py
+-rw-r--r--   0        0        0     1978 2023-06-04 10:45:58.364768 protocol0-1.0.15/protocol0/tests/infra/test_scheduler.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.366760 protocol0-1.0.15/protocol0/tests/shared/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:45:58.368734 protocol0-1.0.15/protocol0/tests/shared/sequence/__init__.py
+-rw-r--r--   0        0        0     1415 2023-06-04 10:45:58.370802 protocol0-1.0.15/protocol0/tests/shared/sequence/test_sanity_sequence.py
+-rw-r--r--   0        0        0     3330 2023-06-04 10:45:58.372490 protocol0-1.0.15/protocol0/tests/shared/sequence/test_sequence.py
+-rw-r--r--   0        0        0     1712 2023-06-04 10:45:58.374260 protocol0-1.0.15/protocol0/tests/shared/sequence/test_sequence_parallel.py
+-rw-r--r--   0        0        0      565 2023-06-04 10:45:58.376262 protocol0-1.0.15/protocol0/tests/shared/test_container.py
+-rw-r--r--   0        0        0     1912 2023-06-08 14:35:44.466357 protocol0-1.0.15/pyproject.toml
+-rw-r--r--   0        0        0     5760 2023-06-08 14:33:21.179852 protocol0-1.0.15/README.md
+-rw-r--r--   0        0        0     6606 1970-01-01 00:00:00.000000 protocol0-1.0.15/PKG-INFO
```

### Comparing `protocol0-1.0.13/LICENSE.md` & `protocol0-1.0.15/LICENSE.md`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command/ScrollScenePositionCommand.py` & `protocol0-1.0.15/protocol0/application/command/ScrollScenePositionCommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from protocol0.application.command.SerializableCommand import SerializableCommand
 
 
 class ScrollScenePositionCommand(SerializableCommand):
     def __init__(self, go_next=False, use_fine_scrolling=False):
         # type: (bool, bool) -> None
         """
-            go_next == True: go right
-            use_fine_scrolling True: scroll by beat instead of bars
+        go_next == True: go right
+        use_fine_scrolling True: scroll by beat instead of bars
         """
         super(ScrollScenePositionCommand, self).__init__()
         self.go_next = go_next
         self.use_fine_scrolling = use_fine_scrolling
```

### Comparing `protocol0-1.0.13/protocol0/application/command/SerializableCommand.py` & `protocol0-1.0.15/protocol0/application/command/SerializableCommand.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/BounceTrackToAudioCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/LoadMatchingTrackCommandHandler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from protocol0.application.command.BounceTrackToAudioCommand import BounceTrackToAudioCommand
+from protocol0.application.command.LoadMatchingTrackCommand import LoadMatchingTrackCommand
 from protocol0.application.command_handler.CommandHandlerInterface import CommandHandlerInterface
-from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackService import \
-    MatchingTrackService
+from protocol0.domain.lom.track.simple_track.audio.SimpleAudioTrack import SimpleAudioTrack
+from protocol0.shared.Song import Song
 
 
-class BounceTrackToAudioCommandHandler(CommandHandlerInterface):
+class LoadMatchingTrackCommandHandler(CommandHandlerInterface):
     def handle(self, command):
-        # type: (BounceTrackToAudioCommand) -> None
-        self._container.get(MatchingTrackService).bounce_current_track()
+        # type: (LoadMatchingTrackCommand) -> None
+        Song.selected_track(SimpleAudioTrack).load_full_track()
```

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/CheckAudioExportValidCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/CheckAudioExportValidCommandHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,11 +4,13 @@
 from protocol0.shared.Song import Song
 from protocol0.shared.logging.Logger import Logger
 
 
 class CheckAudioExportValidCommandHandler(CommandHandlerInterface):
     def handle(self, command):
         # type: (CheckAudioExportValidCommand) -> None
-        sound_id_device = Song.master_track().devices.get_one_from_enum(DeviceEnum.SOUNDID_REFERENCE_PLUGIN)
+        sound_id_device = Song.master_track().devices.get_one_from_enum(
+            DeviceEnum.SOUNDID_REFERENCE_PLUGIN
+        )
         if sound_id_device is not None and sound_id_device.is_enabled:
             sound_id_device.is_enabled = False
             Logger.warning("Deactivating SoundID Reference plugin for export")
```

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/DrumRackToSimplerCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/DrumRackToSimplerCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/EmitBackendEventCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/EmitBackendEventCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/FireSceneToPositionCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/FireSceneToPositionCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/FireSelectedSceneCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/FireSelectedSceneCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/LoadDeviceCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/LoadDeviceCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/LoadDrumRackCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/LoadDrumRackCommandHandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,9 +5,10 @@
 from protocol0.shared.sequence.Sequence import Sequence
 
 
 class LoadDrumRackCommandHandler(CommandHandlerInterface):
     def handle(self, command):
         # type: (LoadDrumRackCommand) -> Sequence
         return self._container.get(TrackFactory).add_sample_track(
-            SampleCategoryEnum.from_value(command.sample_category.upper()), command.sample_subcategory
+            SampleCategoryEnum.from_value(command.sample_category.upper()),
+            command.sample_subcategory,
         )
```

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/LoadMinitaurCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/LoadMinitaurCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/LoadRev2CommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/LoadRev2CommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/MidiNoteCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/MidiNoteCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/RecordUnlimitedCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/RecordUnlimitedCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/ReloadScriptCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/ReloadScriptCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/ScrollScenePositionCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/ScrollScenePositionCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/SelectOrLoadDeviceCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/SelectOrLoadDeviceCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/SelectTrackCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/SelectTrackCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/command_handler/ShowInstrumentCommandHandler.py` & `protocol0-1.0.15/protocol0/application/command_handler/ShowInstrumentCommandHandler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/CommandBus.py` & `protocol0-1.0.15/protocol0/application/CommandBus.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/CommandBusHistory.py` & `protocol0-1.0.15/protocol0/application/CommandBusHistory.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/Container.py` & `protocol0-1.0.15/protocol0/application/Container.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 import Live
 from _Framework.ControlSurface import ControlSurface
 from typing import Type, Dict, Any
 
 from protocol0.application.CommandBus import CommandBus
 from protocol0.application.ContainerInterface import ContainerInterface
 from protocol0.application.ScriptDisconnectedEvent import ScriptDisconnectedEvent
@@ -37,16 +39,17 @@
 from protocol0.domain.lom.song.components.TempoComponent import TempoComponent
 from protocol0.domain.lom.song.components.TrackComponent import TrackComponent
 from protocol0.domain.lom.song.components.TrackCrudComponent import TrackCrudComponent
 from protocol0.domain.lom.track.TrackAutomationService import TrackAutomationService
 from protocol0.domain.lom.track.TrackFactory import TrackFactory
 from protocol0.domain.lom.track.TrackMapperService import TrackMapperService
 from protocol0.domain.lom.track.TrackService import TrackService
-from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackService import \
-    MatchingTrackService
+from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackService import (
+    MatchingTrackService,
+)
 from protocol0.domain.lom.track.simple_track.SimpleTrackService import SimpleTrackService
 from protocol0.domain.lom.validation.ValidatorFactory import ValidatorFactory
 from protocol0.domain.lom.validation.ValidatorService import ValidatorService
 from protocol0.domain.shared.ApplicationView import ApplicationView
 from protocol0.domain.shared.backend.Backend import Backend
 from protocol0.domain.shared.errors.Protocol0Error import Protocol0Error
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
@@ -70,40 +73,53 @@
 
 class Container(ContainerInterface):
     """Direct DI container"""
 
     def __init__(self, control_surface):
         # type: (ControlSurface) -> None
         self._registry = {}  # type: Dict[Type, Any]
+        logging.info("titi")
 
-        DomainEventBus.subscribe(ScriptDisconnectedEvent, lambda _: self._disconnect())
+        # DomainEventBus.subscribe(ScriptDisconnectedEvent, lambda _: self._disconnect())
 
         live_song = control_surface.song()  # type: Live.Song.Song
+        logging.info("titi")
 
         Logger(LoggerService())
+        logging.info("titi")
         UndoFacade(live_song.begin_undo_step, live_song.end_undo_step)
+        logging.info("titi")
         StatusBar(control_surface.show_message)
+        logging.info("titi")
         Backend(control_surface._send_midi)
+        logging.info("titi")
         ErrorService(live_song)
+        logging.info("titi")
         midi_service = MidiService(control_surface._send_midi)
+        logging.info("titi")
         beat_scheduler = BeatScheduler(live_song)
+        logging.info("titi")
         tick_scheduler = TickScheduler(beat_scheduler, live_song)
+        logging.info("titi")
         Scheduler(tick_scheduler, beat_scheduler)  # setup Scheduler facade
+        logging.info("titi")
 
         # song components
         clip_component = ClipComponent(live_song.view)
         device_component = DeviceComponent(live_song.view)
         playback_component = PlaybackComponent(live_song)
         tempo_component = TempoComponent(live_song)
         quantization_component = QuantizationComponent(live_song, tempo_component)
         recording_component = RecordingComponent(live_song)
         scene_component = SceneComponent(live_song.view)
         scene_crud_component = SceneCrudComponent(
             live_song.create_scene, live_song.duplicate_scene, live_song.delete_scene
         )
+        logging.info("titi")
+
         track_component = TrackComponent(live_song.view)
         track_crud_component = TrackCrudComponent(
             live_song.create_midi_track,
             live_song.create_audio_track,
             live_song.duplicate_track,
             live_song.delete_track,
         )
@@ -111,17 +127,15 @@
         ableton_set = AbletonSet()
 
         CommandBus(self, ableton_set)
 
         session_service = SessionService(
             control_surface.component_guard, control_surface.set_highlighting_session_component
         )
-        ApplicationView(
-            recording_component, control_surface.application().view, session_service
-        )
+        ApplicationView(recording_component, control_surface.application().view, session_service)
 
         browser = control_surface.application().browser
         browser_service = BrowserService(browser, BrowserLoaderService(browser))
         device_display_service = DeviceDisplayService(browser_service)
         instrument_display_service = InstrumentDisplayService(device_display_service)
         device_service = DeviceService(track_crud_component, device_component, browser_service)
         drum_rack_service = DrumRackService(browser_service)
@@ -131,14 +145,16 @@
         track_mapper_service = TrackMapperService(live_song, track_factory)
         track_service = TrackService()
         track_recorder_service = RecordService(
             playback_component,
             scene_crud_component,
             quantization_component,
         )
+        logging.info("titi")
+        Logger.dev("dev titi")
         SimpleTrackService()
         matching_track_service = MatchingTrackService(track_crud_component)
         scene_service = SceneService(live_song, scene_crud_component)
         scene_playback_service = ScenePlaybackService(playback_component)
         PlayingSceneFacade(scene_component)
         validator_service = ValidatorService(ValidatorFactory(browser_service), drum_rack_service)
         set_upgrade_service = SetUpgradeService(validator_service, track_crud_component)
```

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/ActionGroupFactory.py` & `protocol0-1.0.15/protocol0/application/control_surface/ActionGroupFactory.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/ActionGroupInterface.py` & `protocol0-1.0.15/protocol0/application/control_surface/ActionGroupInterface.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 [
                     encoder
                     for encoder in self._multi_encoders
                     if encoder.identifier == multi_encoder.identifier
                 ]
             )
             == 0
-        ), "duplicate multi encoder with id %s" % multi_encoder.identifier
+        ), ("duplicate multi encoder with id %s" % multi_encoder.identifier)
         self._multi_encoders.append(multi_encoder)
         return multi_encoder
 
     def add_encoder(
         self,
         identifier,
         name,
```

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/EncoderAction.py` & `protocol0-1.0.15/protocol0/application/control_surface/EncoderAction.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupClip.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupClip.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupCut.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupCut.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupFix.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupFix.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,11 +17,9 @@
         )
 
         # TRaCK encoder
         self.add_encoder(
             identifier=2,
             name="fix current track",
             filter_active_tracks=True,
-            on_press=lambda: self._container.get(ValidatorService).fix_object(
-                Song.current_track()
-            ),
+            on_press=lambda: self._container.get(ValidatorService).fix_object(Song.current_track()),
         )
```

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupLog.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupLog.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupMain.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupMain.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from typing import Optional
 
 from protocol0.application.control_surface.ActionGroupInterface import ActionGroupInterface
 from protocol0.domain.lom.clip.MidiClip import MidiClip
 from protocol0.domain.lom.set.MixingService import MixingService
 from protocol0.domain.lom.song.components.TempoComponent import TempoComponent
 from protocol0.domain.lom.track.TrackAutomationService import TrackAutomationService
-from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackService import \
-    MatchingTrackService
+from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackService import (
+    MatchingTrackService,
+)
 from protocol0.domain.track_recorder.RecordService import RecordService
 from protocol0.domain.track_recorder.RecordTypeEnum import RecordTypeEnum
 from protocol0.shared.Song import Song
 from protocol0.shared.sequence.Sequence import Sequence
 
 
 # noinspection SpellCheckingInspection
@@ -47,15 +48,17 @@
         )
 
         # AUTOmation encoder
         self.add_encoder(
             identifier=3,
             name="automation",
             on_press=self._container.get(TrackAutomationService).color_clip_with_automation,
-            on_long_press=lambda: self._container.get(TrackAutomationService).select_or_sync_automation,
+            on_long_press=lambda: self._container.get(
+                TrackAutomationService
+            ).select_or_sync_automation,
         )
 
         # VOLume encoder
         self.add_encoder(
             identifier=4,
             name="volume",
             on_scroll=self._container.get(MixingService).scroll_all_tracks_volume,
```

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupSample.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupSample.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupSet.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupSet.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/ActionGroupTest.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/ActionGroupTest.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,9 @@
         if isinstance(Song.selected_clip(), AudioClip):
             track = Song.selected_track(SimpleAudioTrack)
             Logger.info(track.clip_mapping._file_path_mapping)
 
     def action_test(self):
         # type: () -> None
         from protocol0.shared.logging.Logger import Logger
+
         Logger.dev("test !")
```

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/group/legacy/ActionGroupPreset.py` & `protocol0-1.0.15/protocol0/application/control_surface/group/legacy/ActionGroupPreset.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/control_surface/MultiEncoder.py` & `protocol0-1.0.15/protocol0/application/control_surface/MultiEncoder.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/error/ErrorService.py` & `protocol0-1.0.15/protocol0/application/error/ErrorService.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     _IGNORED_ERROR_FILENAMES = ("\\venv\\", "\\sequence\\", "\\decorators.py")
 
     def __init__(self, song):
         # type: (Live.Song.Song) -> None
         self._song = song
 
         if self._SET_EXCEPTHOOK:
-            sys.excepthook = self._handle_uncaught_exception
+            sys.excepthook = self._handle_uncaught_exception  # type: ignore[assignment]
 
         DomainEventBus.subscribe(ErrorRaisedEvent, self._on_error_raised_event)
         DomainEventBus.subscribe(BackendEvent, self._on_backend_event)
 
     def _on_error_raised_event(self, event):
         # type: (ErrorRaisedEvent) -> None
         UndoFacade.end_undo_step()
```

### Comparing `protocol0-1.0.13/protocol0/application/Protocol0.py` & `protocol0-1.0.15/protocol0/application/Protocol0.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from _Framework.ControlSurface import ControlSurface
 from typing import Any
 
 from protocol0.application.CommandBus import CommandBus
 from protocol0.application.Container import Container
 from protocol0.application.ScriptDisconnectedEvent import ScriptDisconnectedEvent
 from protocol0.application.ScriptResetActivatedEvent import ScriptResetActivatedEvent
@@ -13,28 +15,30 @@
 from protocol0.shared.sequence.Sequence import Sequence
 
 
 class Protocol0(ControlSurface):
     def __init__(self, c_instance=None):
         # type: (Any) -> None
         super(Protocol0, self).__init__(c_instance=c_instance)
+
         self._initialize()
 
     def _initialize(self, reset=False):
         # type: (bool) -> None
         if reset:
             self.disconnect(reset)
 
         # noinspection PyBroadException
         try:
             Container(self)
         except Exception as e:
             print(e)
             DomainEventBus.emit(ErrorRaisedEvent())
             return
+        logging.info("container saved")
 
         DomainEventBus.subscribe(ScriptResetActivatedEvent, lambda _: self._initialize(reset=True))
         CommandBus.dispatch(ReloadScriptCommand())
 
         Logger.info("P0 script loaded")
 
     def disconnect(self, reset=False):
```

### Comparing `protocol0-1.0.13/protocol0/application/Protocol0Midi.py` & `protocol0-1.0.15/protocol0/application/Protocol0Midi.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,23 @@
         # type: (Any, bool) -> None
         # hide initializing message
         log_message = self.log_message
         self.log_message = lambda a: True
         super(Protocol0Midi, self).__init__(c_instance=c_instance)
         self.log_message = log_message
         # stop log duplication
-        self._c_instance.log_message = MethodType(
-            lambda s, message: None, self._c_instance
-        )  # noqa
+        self._c_instance.log_message = MethodType(lambda s, message: None, self._c_instance)  # noqa
         self.main_p0_script = find_if(
             lambda s: isinstance(s, Protocol0), get_control_surfaces()
         )  # type: Protocol0
 
         self._logger = LoggerService()
 
         if self.main_p0_script is None:
-            self._logger.log(
-                "Error: couldn't find main Protocol0 script", level=LogLevelEnum.ERROR
-            )
+            self._logger.log("Error: couldn't find main Protocol0 script", level=LogLevelEnum.ERROR)
             return
 
         DomainEventBus.subscribe(MidiBytesSentEvent, self._on_midi_bytes_sent_event)
 
     def receive_midi(self, midi_bytes):
         # type: (Tuple) -> None
         DomainEventBus.emit(MidiBytesReceivedEvent(midi_bytes))
```

### Comparing `protocol0-1.0.13/protocol0/application/push2/P0Push2.py` & `protocol0-1.0.15/protocol0/application/push2/P0Push2.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/push2/P0SessionRingTrackProvider.py` & `protocol0-1.0.15/protocol0/application/push2/P0SessionRingTrackProvider.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,9 +95,11 @@
         clamped_offset = min(self.track_offset, max_index)
         if clamped_offset != self.track_offset:
             self.track_offset = clamped_offset
 
     def disconnect(self):
         # type: () -> None
         super(P0SessionRingTrackProvider, self).disconnect()
-        DomainEventBus.un_subscribe(SelectedTrackChangedEvent, self._on_selected_track_changed_event)
+        DomainEventBus.un_subscribe(
+            SelectedTrackChangedEvent, self._on_selected_track_changed_event
+        )
         DomainEventBus.un_subscribe(SessionUpdatedEvent, self._on_session_updated_event)
```

### Comparing `protocol0-1.0.13/protocol0/application/push2/P0ShowInstrumentMode.py` & `protocol0-1.0.15/protocol0/application/push2/P0ShowInstrumentMode.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/application/push2/P0TrackListComponent.py` & `protocol0-1.0.15/protocol0/application/push2/P0TrackListComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/audit/AudioLatencyAnalyzerService.py` & `protocol0-1.0.15/protocol0/domain/audit/AudioLatencyAnalyzerService.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,20 +90,16 @@
         seq.add(partial(track.midi_track.clips[0].set_notes, notes))
         return seq.done()
 
     def _record_test_clip(self):
         # type: () -> Sequence
         track = Song.current_external_synth_track()
         seq = Sequence()
-        seq.add(
-            partial(self._track_recorder_service.record_track, track, RecordTypeEnum.AUDIO)
-        )
-        seq.add(
-            lambda: track.audio_track.clip_slots[0].select()
-        )
+        seq.add(partial(self._track_recorder_service.record_track, track, RecordTypeEnum.AUDIO))
+        seq.add(lambda: track.audio_track.clip_slots[0].select())
         seq.add(partial(CommandBus.dispatch, ResetPlaybackCommand()))
         seq.wait(10)
         return seq.done()
 
     def _analyze_jitter(self):
         # type: () -> Sequence
         track = Song.current_external_synth_track()
```

### Comparing `protocol0-1.0.13/protocol0/domain/audit/LogService.py` & `protocol0-1.0.15/protocol0/domain/audit/LogService.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from protocol0.domain.audit.utils import tail_logs
 from protocol0.domain.lom.clip.AudioClip import AudioClip
 from protocol0.domain.lom.device.DeviceEnum import DeviceEnum
 from protocol0.domain.lom.set.AbletonSet import AbletonSet
 from protocol0.domain.lom.track.TrackMapperService import TrackMapperService
-from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackService import \
-    MatchingTrackService
+from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackService import (
+    MatchingTrackService,
+)
 from protocol0.domain.shared.utils.list import find_if
 from protocol0.shared.Song import Song
 from protocol0.shared.logging.Logger import Logger
 
 
 class LogService(object):
     def __init__(self, ableton_set, track_mapper_service, matching_track_service):
@@ -62,15 +63,18 @@
             Logger.info()
         Logger.info(
             "selected_track.abstract_group_track: %s" % Song.selected_track().abstract_group_track
         )
         Logger.info()
         Logger.info("selected_track.sub_tracks: %s" % Song.selected_track().sub_tracks)
         Logger.info()
-        Logger.info("matching_track: %s" % self._matching_track_service._create_matching_track(Song.selected_track()))
+        Logger.info(
+            "matching_track: %s"
+            % self._matching_track_service._create_matching_track(Song.selected_track())
+        )
         Logger.info()
         Logger.info("selected_track.clip_slots: %s" % Song.selected_track().clip_slots)
         Logger.info()
         Logger.info("selected_track.clips: %s" % Song.selected_track().clips)
         Logger.info()
         Logger.info("selected_track.instrument: %s" % Song.selected_track().instrument)
         if Song.selected_track().instrument:
```

### Comparing `protocol0-1.0.13/protocol0/domain/audit/LOMAnalyzerService.py` & `protocol0-1.0.15/protocol0/domain/audit/LOMAnalyzerService.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,13 +17,15 @@
             if simple_track.is_foldable:
                 for sub_track in simple_track.sub_tracks:
                     assert sub_track.group_track == simple_track, "failed on %s" % simple_track
 
             # 2nd layer checks
             abstract_group_track = simple_track.abstract_group_track
             if simple_track.is_foldable:
-                assert len(abstract_group_track.sub_tracks) == len(simple_track.sub_tracks), "sub tracks inconsistency"
+                assert len(abstract_group_track.sub_tracks) == len(
+                    simple_track.sub_tracks
+                ), "sub tracks inconsistency"
                 for sub_track in abstract_group_track.sub_tracks:
                     if isinstance(sub_track, AbstractGroupTrack):
                         assert sub_track.group_track == abstract_group_track, (
                             "failed on %s" % simple_track
                         )
```

### Comparing `protocol0-1.0.13/protocol0/domain/audit/SetFixerService.py` & `protocol0-1.0.15/protocol0/domain/audit/SetFixerService.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,15 @@
             Logger.warning("Devices to remove: %s" % devices_to_remove)
 
     def _refresh_objects_appearance(self):
         # type: () -> None
         clip_slots = [cs for track in Song.simple_tracks() for cs in track.clip_slots]
         clips = [clip for track in Song.simple_tracks() for clip in track.clips]
         # noinspection PyTypeChecker
-        objects_to_refresh_appearance = (
-                clip_slots + clips + Song.scenes()
-        )
+        objects_to_refresh_appearance = clip_slots + clips + Song.scenes()
 
         for obj in objects_to_refresh_appearance:
             obj.appearance.refresh()
 
         for track in Song.external_synth_tracks():
             track.midi_track.name = "m"
             track.audio_track.name = "a"
```

### Comparing `protocol0-1.0.13/protocol0/domain/audit/SetUpgradeService.py` & `protocol0-1.0.15/protocol0/domain/audit/SetUpgradeService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/audit/stats/ClipStats.py` & `protocol0-1.0.15/protocol0/domain/audit/stats/ClipStats.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/audit/stats/DeviceStats.py` & `protocol0-1.0.15/protocol0/domain/audit/stats/DeviceStats.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 class DevicesStats(object):
     _EXCLUDED_DEVICE_NAMES = [
         DeviceEnum.USAMO.value,
         DeviceEnum.EXTERNAL_AUDIO_EFFECT.value,
         DeviceEnum.SOUNDID_REFERENCE_PLUGIN.value,
-        "Instrument Rack"
+        "Instrument Rack",
     ]
 
     def __init__(self):
         # type: () -> None
         devices = list(self._get_devices())
         device_stats_dict = {}  # type: Dict[str, DeviceStats]
 
@@ -63,15 +63,15 @@
         self.kontakt_instances = len([d for d in devices if d.enum == DeviceEnum.KONTAKT])
 
     def _get_devices(self):
         # type: () -> Iterator[Device]
         """Return only devices that matters for stats"""
 
         for track in Song.all_simple_tracks():
-            for device in track.devices.all:  # type: ignore[has-type]
+            for device in track.devices.all:
                 if (
                     not isinstance(device, (SimplerDevice, DrumRackDevice))
                     and device.type_name not in self._EXCLUDED_DEVICE_NAMES
                 ):
                     yield device
 
     def to_dict(self):
```

### Comparing `protocol0-1.0.13/protocol0/domain/audit/stats/SampleStats.py` & `protocol0-1.0.15/protocol0/domain/audit/stats/SampleStats.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/audit/stats/SceneStats.py` & `protocol0-1.0.15/protocol0/domain/audit/stats/SceneStats.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/audit/stats/SongStats.py` & `protocol0-1.0.15/protocol0/domain/audit/stats/SongStats.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/audit/stats/TrackStats.py` & `protocol0-1.0.15/protocol0/domain/audit/stats/TrackStats.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/AudioClip.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/AudioClip.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/automation/ClipAutomation.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/automation/ClipAutomation.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/automation/ClipAutomationEnvelope.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/automation/ClipAutomationEnvelope.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/Clip.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/Clip.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/ClipAppearance.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/ClipAppearance.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/ClipInfo.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/ClipInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,17 @@
         # type: (List[Clip], List[DeviceParameter], bool) -> List["ClipInfo"]
         unique_clips_by_hash = {}  # type: Dict[float, List[Clip]]
 
         for clip in clips:
             clip_hash = clip.get_hash(device_parameters)
             unique_clips_by_hash[clip_hash] = unique_clips_by_hash.get(clip_hash, []) + [clip]
 
-        clip_infos = [cls(clips[0], device_parameters, clips[1:]) for clips in unique_clips_by_hash.values()]
+        clip_infos = [
+            cls(clips[0], device_parameters, clips[1:]) for clips in unique_clips_by_hash.values()
+        ]
 
         if clean_duplicates:
             for clips in unique_clips_by_hash.values():
                 for clip in clips[1:]:
                     clip.delete()
 
         return clip_infos
@@ -74,24 +76,23 @@
             if dest_clip is None:
                 return False
 
             clip_mapping = dest_track.clip_mapping
 
             if self._DEBUG:
                 hashes = clip_mapping._file_path_mapping.get(dest_clip.file_path, None)
-                Logger.info("Comparing %s to %s : (%s, %s)" % (self, dest_cs, basename(dest_clip.file_path), hashes))
-
+                Logger.info(
+                    "Comparing %s to %s : (%s, %s)"
+                    % (self, dest_cs, basename(dest_clip.file_path), hashes)
+                )
 
             return clip_mapping.path_matches_hash(dest_clip.file_path, self.hash, exact_match)
 
-
         return [cs for cs in track.clip_slots if matches_clip_slot(track, cs, exact_match=exact)]
 
-
-
     @classmethod
     def restore_duplicate_clips(cls, clip_infos):
         # type: (List["ClipInfo"]) -> Sequence
         seq = Sequence()
         for clip_info in clip_infos:
             seq.add(partial(clip_info.restore_duplicates, Song.selected_track()))
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/ClipLoop.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/ClipLoop.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/ClipName.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/ClipName.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/ClipPlayingPosition.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/ClipPlayingPosition.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self._clip_loop = clip_loop
 
     def __repr__(self):
         # type: () -> str
         return "position: %s / %s. beats left: %s" % (
             self.position,
             self._clip_loop.length,
-            self.beats_left
+            self.beats_left,
         )
 
     @property
     def position(self):
         # type: () -> float
         return self._live_clip.playing_position - self._clip_loop.start_marker
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/ClipTail.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/ClipTail.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 
         clip_slots = list(self._track_clip_slots)
         scene_index = playing_scene.index
 
         # activate tail only if the next clip slot is empty
         try:
             has_empty_next_cs = (
-                clip_slots[scene_index + 1].clip is None
-                or clip_slots[scene_index + 1].clip.muted
+                clip_slots[scene_index + 1].clip is None or clip_slots[scene_index + 1].clip.muted
             )
         except IndexError:
             return
 
         # let the tail play
         if (
             has_empty_next_cs
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip/MidiClip.py` & `protocol0-1.0.15/protocol0/domain/lom/clip/MidiClip.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip_slot/AudioClipSlot.py` & `protocol0-1.0.15/protocol0/domain/lom/clip_slot/AudioClipSlot.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip_slot/ClipSlot.py` & `protocol0-1.0.15/protocol0/domain/lom/clip_slot/ClipSlot.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         # type: () -> Sequence
         seq = Sequence()
         if self._clip_slot and self.has_clip and self.clip:
             seq.add(self._clip_slot.delete_clip)
             seq.wait_for_event(ClipCreatedOrDeletedEvent, self._clip_slot)
         return seq.done()
 
-
     def prepare_for_record(self):
         # type: () -> Sequence
         seq = Sequence()
         if self.clip:
             seq.add(self.delete_clip)
             seq.wait(3)  # because has stop button is automatically removed on deletion
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/clip_slot/ClipSlotAppearance.py` & `protocol0-1.0.15/protocol0/domain/lom/clip_slot/ClipSlotAppearance.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/Device.py` & `protocol0-1.0.15/protocol0/domain/lom/device/Device.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         self._view = self._device.view  # type: Live.Device.Device.View
         self.parameters = []  # type: List[DeviceParameter]
         self._parameters_listener.subject = self._device
         self._parameters_listener()
         self.can_have_drum_pads = self._device.can_have_drum_pads  # type: bool
         self.can_have_chains = self._device.can_have_chains  # type: bool
 
-
     def __repr__(self):
         # type: () -> str
         return "%s(%s)" % (self.__class__.__name__, smart_string(self.name))
 
     @classmethod
     def _get_class(cls, device):
         # type: (Any) -> Type[Device]
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DeviceChain.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DeviceChain.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DeviceDisplayService.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DeviceDisplayService.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,17 +85,15 @@
                 d.is_collapsed = True
         for d in parent_rack.chains[0].devices:
             if not d.is_collapsed:
                 devices_to_un_collapse.append(d)
                 d.is_collapsed = True
 
         rack_coords = self._get_rack_show_macros_button_click_coordinates(track, parent_rack)
-        device_coords = self._get_device_show_button_click_coordinates(
-            track, device, parent_rack
-        )
+        device_coords = self._get_device_show_button_click_coordinates(track, device, parent_rack)
 
         seq = Sequence()
         seq.add(partial(self._toggle_ableton_button, rack_coords, activate=False))
         seq.wait(5)
         seq.add(partial(self._toggle_ableton_button, device_coords, activate=activate))
         seq.wait(10)
         seq.add(partial(self._toggle_ableton_button, rack_coords, activate=True))
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DeviceEnum.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DeviceEnum.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DeviceEnumGroup.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DeviceEnumGroup.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,11 +12,8 @@
 
     def __repr__(self):
         # type: () -> str
         return "DeviceEnumGroup('%s')" % self.name
 
     def to_dict(self):
         # type: () -> Dict
-        return {
-            "name": self.name,
-            "devices": [d.name for d in self.enums]
-        }
+        return {"name": self.name, "devices": [d.name for d in self.enums]}
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DeviceService.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DeviceService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DrumPad.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DrumPad.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         if self.is_empty:
             out += ", empty=True"
         return out + ")"
 
     @subject_slot("chains")
     def _chains_listener(self):
         # type: () -> None
-        self.chains = [DeviceChain(chain, index) for index, chain in enumerate(self._drum_pad.chains)]
+        self.chains = [
+            DeviceChain(chain, index) for index, chain in enumerate(self._drum_pad.chains)
+        ]
 
     @property
     def name(self):
         # type: () -> str
         return smart_string(self._drum_pad.name)
 
     @property
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DrumRackDevice.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DrumRackDevice.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DrumRackSampleService.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DrumRackSampleService.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from protocol0.domain.lom.device.DrumRackDevice import DrumRackDevice
 from protocol0.domain.lom.device.Sample.Sample import Sample
 from protocol0.domain.lom.instrument.instrument.InstrumentDrumRack import InstrumentDrumRack
 from protocol0.domain.lom.track.simple_track.SimpleTrack import SimpleTrack
 from protocol0.domain.shared.errors.Protocol0Warning import Protocol0Warning
 from protocol0.shared.Song import Song
 
+
 def _get_drum_rack(track):
     # type: (SimpleTrack) -> DrumRackDevice
     if not isinstance(track.instrument, InstrumentDrumRack):
         raise Protocol0Warning("track has no drum rack")
 
     return cast(DrumRackDevice, track.instrument.device)
 
+
 def _get_selected_sample(track):
     # type: (SimpleTrack) -> Sample
     drum_rack = _get_drum_rack(track)
 
     return drum_rack.selected_drum_pad.sample
 
+
 class DrumRackSampleService(object):
     def warp_selected_sample(self):
         # type: () -> None
         sample = _get_selected_sample(Song.selected_track())
         sample.warping = not sample.warping
 
     def warp_all(self):
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/DrumRackService.py` & `protocol0-1.0.15/protocol0/domain/lom/device/DrumRackService.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import itertools
 from functools import partial
-
 from typing import cast, Optional
 
 from protocol0.domain.lom.clip.MidiClip import MidiClip
 from protocol0.domain.lom.device.DeviceEnum import DeviceEnum
 from protocol0.domain.lom.device.DrumPad import DrumPad
 from protocol0.domain.lom.device.DrumRackDevice import DrumRackDevice
 from protocol0.domain.lom.device.DrumRackLoadedEvent import DrumRackLoadedEvent
@@ -74,15 +72,15 @@
         assert len(device.filled_drum_pads) == 0, "device has drum pads"
         presets = drum_category.presets
         drum_pads = [d for d in device.drum_pads if d.note >= DrumPad.INITIAL_NOTE][: len(presets)]
 
         seq = Sequence()
         seq.add(DrumPad.select_first_pad)
 
-        for drum_pad, preset in itertools.izip(drum_pads, presets):
+        for drum_pad, preset in zip(drum_pads, presets):
             seq.add(partial(setattr, device, "selected_drum_pad", drum_pad))
             seq.add(partial(self._browser_service.load_drum_pad_sample, preset.original_name))
             seq.wait(3)
 
         seq.wait(20)
         # seq.add(partial(Backend.client().save_drum_rack, drum_category.drum_rack_name))
         return seq.done()
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/MixerDevice.py` & `protocol0-1.0.15/protocol0/domain/lom/device/MixerDevice.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,23 +7,19 @@
 
 class MixerDevice(SlotManager):
     def __init__(self, live_mixer_device):
         # type: (Live.MixerDevice.MixerDevice) -> None
         super(MixerDevice, self).__init__()
 
         parameters = live_mixer_device.sends + [live_mixer_device.volume, live_mixer_device.panning]
-        self._parameters = [
-            DeviceParameter(parameter) for parameter in parameters
-        ]
+        self._parameters = [DeviceParameter(parameter) for parameter in parameters]
 
     def to_dict(self):
         # type: () -> Dict
-        return {
-            "params": [p.value for p in self.parameters]
-        }
+        return {"params": [p.value for p in self.parameters]}
 
     def update_from_dict(self, mixer_data):
         # type: (Dict) -> None
         assert len(self.parameters) == len(mixer_data["params"]), "Cannot update mixer device"
         for param, value in zip(self.parameters, mixer_data["params"]):
             param.value = value
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/PluginDevice.py` & `protocol0-1.0.15/protocol0/domain/lom/device/PluginDevice.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/RackDevice.py` & `protocol0-1.0.15/protocol0/domain/lom/device/RackDevice.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/Sample/Sample.py` & `protocol0-1.0.15/protocol0/domain/lom/device/Sample/Sample.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/SimplerDevice.py` & `protocol0-1.0.15/protocol0/domain/lom/device/SimplerDevice.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             Live.SimplerDevice.SimplerDevice, self._device
         )  # type: Live.SimplerDevice.SimplerDevice
         self._sample = Sample(self._device.sample)
         Scheduler.defer(self._set_warping)
 
     def __repr__(self):
         # type: () -> str
-        return "SimplerDevice(name=%s, sample=%s)" % (self.name.encode('utf-8'), "test")
+        return "SimplerDevice(name=%s, sample=%s)" % (self.name, "test")
 
     @property
     def sample(self):
         # type: () -> Sample
         return self._sample
 
     @property
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device/SimpleTrackDevices.py` & `protocol0-1.0.15/protocol0/domain/lom/device/SimpleTrackDevices.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device_parameter/DeviceParameter.py` & `protocol0-1.0.15/protocol0/domain/lom/device_parameter/DeviceParameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,25 +122,24 @@
         param.value = value
 
     @accelerate
     def scroll(self, go_next, factor=1):
         # type: (bool, int) -> None
         # using factor acceleration
         value_range = self.max - self.min
-        step = (value_range / 1000)
+        step = value_range / 1000
         step *= factor
         value = self.value + step if go_next else self.value - step
         self.value = clamp(value, self.min, self.max)
 
     def reset(self):
         # type: () -> None
         if self.name == "Device On":
             # we define arbitrarily that toggling a device always starts from disabled state
             # not the opposite
             self.value = 0
         else:
-
             try:
                 self.value = self.default_value
             except RuntimeError as e:
                 Logger.error((e, self, self.device_name, self.min, self.max, self.default_value))
                 raise e
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device_parameter/DeviceParameterEnum.py` & `protocol0-1.0.15/protocol0/domain/lom/device_parameter/DeviceParameterEnum.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device_parameter/DeviceParameterValue.py` & `protocol0-1.0.15/protocol0/domain/lom/device_parameter/DeviceParameterValue.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/device_parameter/LinkedDeviceParameters.py` & `protocol0-1.0.15/protocol0/domain/lom/device_parameter/LinkedDeviceParameters.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentAddictiveKeys.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentAddictiveKeys.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentMinitaur.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentMinitaur.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentRev2.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentRev2.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,15 @@
         # type: (Any, Any) -> None
         super(InstrumentRev2, self).__init__(*a, **k)
 
         DomainEventBus.subscribe(SimpleTrackArmedEvent, self._on_simple_track_armed_event)
         DomainEventBus.subscribe(
             ExtAudioRecordingStartedEvent, self._on_audio_recording_started_event
         )
-        DomainEventBus.subscribe(
-            ExtAudioRecordingEndedEvent, self._on_audio_recording_ended_event
-        )
+        DomainEventBus.subscribe(ExtAudioRecordingEndedEvent, self._on_audio_recording_ended_event)
 
     @property
     def needs_exclusive_activation(self):
         # type: () -> bool
         return InstrumentRev2.ACTIVE_INSTANCE != self
 
     def exclusive_activate(self):
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/instrument/InstrumentSimpler.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/instrument/InstrumentSimpler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentDisplayService.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentDisplayService.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from protocol0.domain.lom.instrument.InstrumentSelectedEvent import InstrumentSelectedEvent
 from protocol0.domain.lom.track.abstract_track.AbstractTrack import AbstractTrack
 from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import (
     ExternalSynthTrack,
 )
 from protocol0.domain.lom.track.simple_track.SimpleTrack import SimpleTrack
 from protocol0.domain.lom.track.simple_track.SimpleTrackArmedEvent import SimpleTrackArmedEvent
-from protocol0.domain.lom.track.simple_track.SimpleTrackSaveStartedEvent import \
-    SimpleTrackSaveStartedEvent
+from protocol0.domain.lom.track.simple_track.SimpleTrackSaveStartedEvent import (
+    SimpleTrackSaveStartedEvent,
+)
 from protocol0.domain.shared.backend.Backend import Backend
 from protocol0.domain.shared.errors.Protocol0Warning import Protocol0Warning
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
 from protocol0.shared.Song import Song
 from protocol0.shared.logging.Logger import Logger
 from protocol0.shared.sequence.Sequence import Sequence
 
@@ -24,15 +25,17 @@
 
 
 class InstrumentDisplayService(object):
     def __init__(self, device_display_service):
         # type: (DeviceDisplayService) -> None
         self._device_display_service = device_display_service
         DomainEventBus.subscribe(SimpleTrackArmedEvent, self._on_simple_track_armed_event)
-        DomainEventBus.subscribe(SimpleTrackSaveStartedEvent, self._on_simple_track_save_started_event)
+        DomainEventBus.subscribe(
+            SimpleTrackSaveStartedEvent, self._on_simple_track_save_started_event
+        )
         DomainEventBus.subscribe(InstrumentSelectedEvent, self._on_instrument_selected_event)
 
     def show_instrument(self, track):
         # type: (AbstractTrack) -> Optional[Sequence]
         if track.instrument is None or not track.instrument.CAN_BE_SHOWN:
             raise Protocol0Warning("Instrument cannot be shown")
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentFactory.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentFactory.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/InstrumentInterface.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/InstrumentInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 
 
 def load_instrument_track(instrument_cls):
     # type: (Type["InstrumentInterface"]) -> Sequence
     insert_track = Song.current_track().base_track
     track_color = insert_track.color
 
-
     seq = Sequence()
     seq.add(insert_track.focus)
     seq.add(partial(Backend.client().load_instrument_track, instrument_cls.INSTRUMENT_TRACK_NAME))
     seq.wait_for_backend_event("instrument_loaded")
     seq.add(partial(setattr, insert_track, "color", track_color))
     seq.defer()
     seq.wait_for_event(TracksMappedEvent)
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/InstrumentPreset.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/InstrumentPreset.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/InstrumentPresetList.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/InstrumentPresetList.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/InstrumentPresetScrollerService.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/InstrumentPresetScrollerService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_changer/InstrumentRackPresetChanger.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_changer/ProgramChangePresetChanger.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_changer/SamplePresetChanger.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/DirectoryPresetImporter.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/FilePresetImporter.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/FilePresetImporter.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/PluginDevicePresetImporter.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/PresetImporterFactory.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from protocol0.domain.lom.device.RackDevice import RackDevice
 from protocol0.domain.lom.instrument.preset.preset_importer.DirectoryPresetImporter import (
     DirectoryPresetImporter,
 )
 from protocol0.domain.lom.instrument.preset.preset_importer.FilePresetImporter import (
     FilePresetImporter,
 )
-from protocol0.domain.lom.instrument.preset.preset_importer.NullPresetImporter import \
-    NullPresetImporter
+from protocol0.domain.lom.instrument.preset.preset_importer.NullPresetImporter import (
+    NullPresetImporter,
+)
 from protocol0.domain.lom.instrument.preset.preset_importer.PluginDevicePresetImporter import (
     PluginDevicePresetImporter,
 )
 from protocol0.domain.lom.instrument.preset.preset_importer.PresetImportInterface import (
     PresetImportInterface,
 )
 from protocol0.domain.lom.instrument.preset.preset_importer.RackDevicePresetImporter import (
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/PresetImportInterface.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/PresetImportInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_importer/RackDevicePresetImporter.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerDevicePresetName.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerGroupTrackName.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py` & `protocol0-1.0.15/protocol0/domain/lom/instrument/preset/preset_initializer/PresetInitializerInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/loop/LoopableInterface.py` & `protocol0-1.0.15/protocol0/domain/lom/loop/LoopableInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/note/Note.py` & `protocol0-1.0.15/protocol0/domain/lom/note/Note.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,18 +38,15 @@
             self.muted,
         )
 
     @classmethod
     def from_midi_note(cls, note):
         # type: (Live.Clip.MidiNote) -> Note
         return Note(
-            pitch=note.pitch,
-            start=note.start_time,
-            duration=note.duration,
-            velocity=note.velocity
+            pitch=note.pitch, start=note.start_time, duration=note.duration, velocity=note.velocity
         )
 
     def to_data(self):
         # type: () -> Tuple[int, float, float, int, bool]
         return self.pitch, self.start, self.duration, int(self.velocity), self.muted
 
     def _is_value_equal(self, val1, val2, delta=0.00001):
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/sample/SampleCategory.py` & `protocol0-1.0.15/protocol0/domain/lom/sample/SampleCategory.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 from protocol0.domain.lom.track.simple_track.SimpleTrack import SimpleTrack
 from protocol0.domain.shared.backend.Backend import Backend
 from protocol0.shared.Song import Song
 
 
 class SampleCategory(object):
     """
-        Represents a sample folder that can be loaded in one click in a drum rack
+    Represents a sample folder that can be loaded in one click in a drum rack
 
-        Used to access my library easily
+    Used to access my library easily
     """
+
     def __init__(self, category, name):
         # type: (SampleCategoryEnum, str) -> None
         self._category = category
         self._name = name
 
     def __repr__(self):
         # type: () -> str
@@ -51,17 +52,15 @@
     def presets(self):
         # type: () -> List[InstrumentPreset]
         return DirectoryPresetImporter(self._sample_directory).import_presets()
 
     @property
     def live_presets(self):
         # type: () -> List[InstrumentPreset]
-        return DirectoryPresetImporter(self._sample_directory).import_presets(
-            use_cache=False
-        )
+        return DirectoryPresetImporter(self._sample_directory).import_presets(use_cache=False)
 
     @property
     def create_track_index(self):
         # type: () -> int
         assert self._parent_track is not None, "Sample group track doesn't exist"
         sample_tracks = self._parent_track.get_all_simple_sub_tracks()
 
@@ -87,10 +86,10 @@
         if self._category == SampleCategoryEnum.VOCALS and Song.vocals_track() is None:
             Backend.client().show_warning(
                 "Couldn't find %s track. Using drums track instead" % VocalsTrack.TRACK_NAME
             )
             return Song.drums_track()
 
         return {
-                SampleCategoryEnum.DRUMS: Song.drums_track(),
-                SampleCategoryEnum.VOCALS: Song.vocals_track(),
-            }[self._category]
+            SampleCategoryEnum.DRUMS: Song.drums_track(),
+            SampleCategoryEnum.VOCALS: Song.vocals_track(),
+        }[self._category]
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/sample/SampleCategoryEnum.py` & `protocol0-1.0.15/protocol0/domain/lom/sample/SampleCategoryEnum.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/LoopingSceneToggler.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/LoopingSceneToggler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/PlayingSceneFacade.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/PlayingSceneFacade.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         # type: () -> List[Optional[Scene]]
         return cls._INSTANCE._last_playing_scenes
 
     @classmethod
     def _check_for_unknown_playing_scenes(cls):
         # type: () -> None
         """
-            Monitoring method to find out
-            why some scenes are left out of the playing scene pattern
+        Monitoring method to find out
+        why some scenes are left out of the playing scene pattern
         """
         unknown_playing_scenes = []
         for scene in Song.scenes():
             if scene.playing_state.is_playing and scene != cls.get():
                 unknown_playing_scenes.append(scene)
 
         history = list(reversed(cls.history()))
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/Scene.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/Scene.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,17 @@
             else:
                 return next_scene
 
     @property
     def should_loop(self):
         # type: () -> bool
         return (
-                self == Song.looping_scene()
-                or self == Song.scenes()[-1]
-                or Song.scenes()[self.index + 1].bar_length == 0
+            self == Song.looping_scene()
+            or self == Song.scenes()[-1]
+            or Song.scenes()[self.index + 1].bar_length == 0
         )
 
     @property
     def previous_scene(self):
         # type: () -> Scene
         if self == Song.scenes()[0]:
             return self
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/SceneAppearance.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/SceneAppearance.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/SceneClips.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/SceneClips.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/SceneCropScroller.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/SceneCropScroller.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/SceneLength.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/SceneLength.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/SceneName.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/SceneName.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/ScenePlaybackService.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/ScenePlaybackService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/ScenePlayingState.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/ScenePlayingState.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,15 @@
                 return False
             # tail clips of audio tracks
             if isinstance(clip, AudioClip) and clip.bar_length > self._scene_length.bar_length:
                 return False
 
             return True
 
-        return Song.is_playing() and any(
-            _is_clip_playing(clip) for clip in self._clips
-        )
+        return Song.is_playing() and any(_is_clip_playing(clip) for clip in self._clips)
 
     @property
     def position(self):
         # type: () -> float
         longest_clip = self._scene_length.get_longest_clip(is_playing=True)
         if longest_clip is not None:
             return longest_clip.playing_position.position
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/ScenePositionScroller.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/ScenePositionScroller.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def _get_values(self):
         # type: () -> List
         if self.use_fine_scrolling:
             beat_division = 1.0 / Song.signature_numerator()
             return [x * beat_division for x in range(0, int(self._scene_length.length))]
         else:
-            return range(0, self._scene_length.bar_length)
+            return list(range(0, self._scene_length.bar_length))
 
     def _get_initial_value(self, go_next):
         # type: (bool) -> int
         if self._scene_playing_state.is_playing:
             bar_position = self._scene_playing_state.bar_position
             return int(floor(bar_position) if go_next else round(bar_position))
         else:
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/SceneService.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/SceneService.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
 
                 del self._live_scene_id_to_scene[scene_id]
 
             scene.disconnect()
             if scene == Song.playing_scene():
                 PlayingSceneFacade.set(None)
 
-
     def generate_scene(self, live_scene, index):
         # type: (Live.Scene.Scene, int) -> None
         # switching to full remap because of persisting mapping problems when moving scenes
         scene = Scene(live_scene, index)
         self._live_scene_id_to_scene[scene.live_id] = scene
 
     def _sort_scenes(self):
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/scene/SceneWindow.py` & `protocol0-1.0.15/protocol0/domain/lom/scene/SceneWindow.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/set/AbletonSet.py` & `protocol0-1.0.15/protocol0/domain/lom/set/AbletonSet.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,25 +83,23 @@
             "active": self.active,
             "path": self._path,
             "title": self._title,
             "muted": muted,
             "current_track": Song.current_track().to_dict(),
             "selected_track": Song.selected_track().to_dict(),
             "track_count": len(list(Song.simple_tracks())),
-            "drum_rack_visible": isinstance(
-                Song.selected_track().instrument, InstrumentDrumRack
-            ),
+            "drum_rack_visible": isinstance(Song.selected_track().instrument, InstrumentDrumRack),
         }
 
     def notify(self, force=False):
         # type: (bool) -> None
         data = self.to_dict()
         if self._cache != data or force:
             seq = Sequence()
-            seq.add(partial(Backend.client().notify_set_state, data))
+            seq.add(partial(Backend.client().post_set, data))
 
             if self._title is None:
                 seq.wait_for_backend_event("set_updated")
                 seq.add(lambda: self._set_from_server_response(seq.res))  # type: ignore[arg-type]
 
             seq.done()
 
@@ -117,13 +115,15 @@
         self._path = res["path"]
 
         if not self.is_unknown and not self.is_test:
             abstract_track_names = [t.name for t in Song.abstract_tracks()]
             orphan_tracks = [t for t in self._saved_tracks if t not in abstract_track_names]
 
             if len(orphan_tracks):
-                Backend.client().show_warning("Found orphan saved tracks: \n\n%s" % "\n".join(orphan_tracks))
+                Backend.client().show_warning(
+                    "Found orphan saved tracks: \n\n%s" % "\n".join(orphan_tracks)
+                )
                 Backend.client().show_saved_tracks()
 
     def _disconnect(self):
         # type: () -> None
         Backend.client().close_set(self._id)
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/set/SessionToArrangementService.py` & `protocol0-1.0.15/protocol0/domain/lom/set/SessionToArrangementService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/ClipComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/ClipComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/DeviceComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/DeviceComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/PlaybackComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/PlaybackComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/QuantizationComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/QuantizationComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/RecordingComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/RecordingComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/SceneComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/SceneComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/SceneCrudComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/SceneCrudComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/TempoComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/TempoComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/TrackComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/TrackComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/components/TrackCrudComponent.py` & `protocol0-1.0.15/protocol0/domain/lom/song/components/TrackCrudComponent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/song/SongInitService.py` & `protocol0-1.0.15/protocol0/domain/lom/song/SongInitService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/AbstrackTrackArmState.py` & `protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/AbstrackTrackArmState.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,11 +46,10 @@
 
     def arm_track(self):
         # type: () -> Optional[Sequence]
         Logger.warning("Tried arming un-armable track")
 
         return None
 
-
     def unarm(self):
         # type: () -> None
         self.is_armed = False
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/AbstractTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/AbstractTrack.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/abstract_track/AbstractTrackAppearance.py` & `protocol0-1.0.15/protocol0/domain/lom/track/abstract_track/AbstractTrackAppearance.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/AbstractGroupTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/AbstractGroupTrack.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtArmState.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtArmState.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from functools import partial
 
 from typing import Optional
 
 from protocol0.domain.lom.track.abstract_track.AbstrackTrackArmState import AbstractTrackArmState
-from protocol0.domain.lom.track.group_track.ext_track.ExtArmedEvent import \
-    ExtArmedEvent
+from protocol0.domain.lom.track.group_track.ext_track.ExtArmedEvent import ExtArmedEvent
 from protocol0.domain.lom.track.routing.InputRoutingTypeEnum import InputRoutingTypeEnum
 from protocol0.domain.lom.track.simple_track.audio.SimpleAudioTrack import SimpleAudioTrack
 from protocol0.domain.lom.track.simple_track.midi.SimpleMidiTrack import SimpleMidiTrack
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
 from protocol0.shared.sequence.Sequence import Sequence
 
 
@@ -19,18 +18,15 @@
         self._base_track = base_track
         self._sub_tracks = base_track.sub_tracks
         self._midi_track = midi_track
 
     @property
     def is_armed(self):
         # type: () -> bool
-        return all(
-            sub_track.arm_state.is_armed
-            for sub_track in self._sub_tracks
-        )
+        return all(sub_track.arm_state.is_armed for sub_track in self._sub_tracks)
 
     @is_armed.setter
     def is_armed(self, is_armed):
         # type: (bool) -> None
         for track in self._sub_tracks:
             track.arm_state.is_armed = is_armed
 
@@ -41,20 +37,15 @@
 
         self._midi_track.external_device.is_enabled = True
 
         if self._midi_track.input_routing.type == InputRoutingTypeEnum.NO_INPUT:
             self._midi_track.input_routing.type = InputRoutingTypeEnum.ALL_INS
 
         seq = Sequence()
-        seq.add(
-            [
-                sub_track.arm_state.arm_track
-                for sub_track in self._sub_tracks
-            ]
-        )
+        seq.add([sub_track.arm_state.arm_track for sub_track in self._sub_tracks])
         seq.add(self.notify_observers)
         seq.add(partial(DomainEventBus.emit, ExtArmedEvent(self._base_track)))
         return seq.done()
 
     def unarm(self):
         # type: () -> None
         self.is_armed = False
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExternalSynthTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExternalSynthTrack.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtMatchingTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleMatchingTrack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,66 @@
-from typing import cast, Optional
+from typing import Any, Optional
 
 from protocol0.domain.lom.clip.ClipColorEnum import ClipColorEnum
 from protocol0.domain.lom.clip.ClipInfo import ClipInfo
 from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackClipColorManager import (
     MatchingTrackClipColorManager,
 )
 from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackInterface import (
     MatchingTrackInterface,
 )
-from protocol0.domain.lom.track.simple_track.audio.SimpleAudioTrack import SimpleAudioTrack
+from protocol0.domain.lom.track.group_track.matching_track.utils import (
+    assert_valid_track_name,
+    ensure_clips_looped,
+)
+from protocol0.shared.Song import Song
 from protocol0.shared.sequence.Sequence import Sequence
 
 
-class ExtMatchingTrack(MatchingTrackInterface):
-    def __init__(self, base_track):
-        # type: (SimpleAudioTrack) -> None
-        super(ExtMatchingTrack, self).__init__(base_track)
-        self._midi_sub_track = cast(SimpleAudioTrack, base_track.sub_tracks[0])
-        self._audio_sub_track = cast(SimpleAudioTrack, base_track.sub_tracks[1])
-        # in this setup the mapping is shared between 3 audio tracks
-        self._audio_track.clip_mapping.update(
-            self._audio_sub_track.clip_mapping
-        )
-        self._audio_sub_track.clip_mapping = (
-            self._audio_track.clip_mapping
-        )
+class SimpleMatchingTrack(MatchingTrackInterface):
+    def __init__(self, *a, **k):
+        # type: (Any, Any) -> None
+        super(SimpleMatchingTrack, self).__init__(*a, **k)
+        # clean the mixer if necessary (e.g. when loading back a midi track for the 1st time)
+        self._base_track.reset_mixer()
 
     @property
     def clip_color_manager(self):
         # type: () -> Optional[MatchingTrackClipColorManager]
-        return MatchingTrackClipColorManager(
-            self.router, self._midi_sub_track, self._audio_track, self._audio_sub_track
-        )
+        return MatchingTrackClipColorManager(self.router, self._base_track, self._audio_track)
+
+    def init_clips(self):
+        # type: () -> None
+        for clip in self._base_track.clips:
+            clip.previous_hash = clip.get_hash(self._base_track.devices.parameters)
 
     def bounce(self):
         # type: () -> Optional[Sequence]
-        assert len(list(self._base_track.devices)) == 0, "Please move devices to audio track"
         assert self._base_track.devices.mixer_device.is_default, "Mixer was changed"
+        assert_valid_track_name(self._base_track.name)
+
+        ensure_clips_looped(self._base_track.clips)
+
+        # maintain hash / path link on hash change (update)
+        for clip in self._base_track.clips:
+            clip_hash = clip.get_hash(self._base_track.devices.parameters)
+            if clip.previous_hash == clip_hash:
+                continue
+
+            self._audio_track.clip_mapping.register_hash_equivalence(clip.previous_hash, clip_hash)
+            clip.previous_hash = clip_hash
 
         bounced_clips = [
-            (mc, ac)
-            for (mc, ac) in zip(self._midi_sub_track.clips, self._audio_sub_track.clips)
-            if mc.color == ClipColorEnum.DISABLED.value and ac.color == ClipColorEnum.DISABLED.value
+            c for c in self._base_track.clips if c.color == ClipColorEnum.DISABLED.value
         ]
-        bounced_clips_flat = [c for clips in bounced_clips for c in clips]
-        for clip in bounced_clips_flat:
+        for clip in bounced_clips:
             assert ClipInfo(clip, self._base_track.devices.parameters).already_bounced_to(
                 self._audio_track
-            ), "clip disabled but not bounced: %s" % clip
+            ), ("clip disabled but not bounced: %s" % clip)
 
         seq = Sequence()
-
-        seq.add(self._base_track.abstract_track.arm_state.unarm)
         seq.add(self._base_track.save)
-        seq.add([c.delete for c in bounced_clips_flat])
-        seq.add(self._audio_sub_track.flatten)
-        seq.add(self._base_track.delete)
+        seq.add([c.delete for c in bounced_clips])
+        seq.add(self._base_track.flatten)
+        seq.add(lambda: Song.selected_track().delete())
 
         return seq.done()
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtMatchingTrackCreator.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,9 +58,8 @@
         seq.add(
             lambda: Song.selected_track().devices.mixer_device.update_from_dict(mixer_data)
         )  # noqa
         seq.add(self._audio_track.flatten)
         seq.add(self._base_track.delete)
         seq.add(partial(Backend.client().show_success, "Track bounced"))
 
-
         return seq.done()
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtMonitoringState.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtMonitoringState.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/ExtSoloState.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtSoloState.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/SimpleAudioExtTrack.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/SimpleBaseExtTrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,10 @@
         super(SimpleBaseExtTrack, self).update(observable)
 
         devices_count = len(list(self.devices))
         if devices_count > 0:
             Logger.info("Found %s devices on ext base track %s" % (devices_count, self))
 
             if devices_count == 1:
-                Backend.client().show_warning("Please add this device to the audio sub track", centered=True)
+                Backend.client().show_warning(
+                    "Please add this device to the audio sub track", centered=True
+                )
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/SimpleMidiExtTrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,9 @@
         super(SimpleMidiExtTrack, self).__init__(*a, **k)
         self.clip_tail.active = False
 
     @property
     def external_device(self):
         # type: () -> Optional[Device]
         return find_if(
-            lambda d: d.enum is not None and d.enum.is_external_device,
-            list(self.devices)
+            lambda d: d.enum is not None and d.enum.is_external_device, list(self.devices)
         )
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackClipColorManager.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackClipManager.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackCreatorInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackInterface.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackRouter.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackRouter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,17 @@
             if observable.is_armed:
                 self.monitor_base_track()
             else:
                 self.monitor_audio_track()
 
     def monitor_base_track(self):
         # type: () -> None
-        if not liveobj_valid(self._base_track._track) or not liveobj_valid(self._audio_track._track):
+        if not liveobj_valid(self._base_track._track) or not liveobj_valid(
+            self._audio_track._track
+        ):
             return None
 
         self._audio_track.current_monitoring_state = CurrentMonitoringStateEnum.IN
         self._audio_track.input_routing.type = InputRoutingTypeEnum.NO_INPUT
         self._base_track.output_routing.track = self._audio_track
 
     def monitor_audio_track(self):
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackService.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/MatchingTrackSoloState.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/matching_track/utils.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/matching_track/utils.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/NormalGroupMatchingTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/NormalGroupMatchingTrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import partial
 
 from typing import Optional
 
-from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackClipColorManager import \
-    MatchingTrackClipColorManager
+from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackClipColorManager import (
+    MatchingTrackClipColorManager,
+)
 from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackInterface import (
     MatchingTrackInterface,
 )
 from protocol0.domain.shared.backend.Backend import Backend
 from protocol0.shared.sequence.Sequence import Sequence
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/NormalGroupMatchingTrackCreator.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,13 @@
         self._base_track.reset_mixer()
         seq.add(self._base_track.save)
 
         insert_index = self._base_track.sub_tracks[-1].index + 1
         seq.add(partial(self._track_crud_component.create_audio_track, insert_index))
         seq.add(lambda: setattr(Song.selected_track(), "name", self._base_track.name))
         seq.add(lambda: setattr(Song.selected_track(), "color", self._base_track.color))
-        seq.add(
-            lambda: Song.selected_track().devices.mixer_device.update_from_dict(mixer_data)
-        )
+        seq.add(lambda: Song.selected_track().devices.mixer_device.update_from_dict(mixer_data))
         seq.add(lambda: setattr(Song.selected_track().input_routing, "track", self._base_track))
         seq.add(lambda: Song.selected_track().arm_state.arm())
         seq.add(partial(Backend.client().show_success, "Track created, please record clips"))
 
         return seq.done()
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/group_track/NormalGroupTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/NormalGroupTrack.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 
 class NormalGroupTrack(AbstractGroupTrack):
     @classmethod
     def make(cls, base_group_track):
         # type: (SimpleTrack) -> NormalGroupTrack
         from protocol0.domain.lom.track.group_track.DrumsTrack import DrumsTrack
-        from protocol0.domain.lom.track.simple_track.audio.special.ReferenceTrack import ReferenceTrack
+        from protocol0.domain.lom.track.simple_track.audio.special.ReferenceTrack import (
+            ReferenceTrack,
+        )
         from protocol0.domain.lom.track.group_track.VocalsTrack import VocalsTrack
 
         if DrumsTrack.is_track_valid(base_group_track):
             return DrumsTrack(base_group_track)
         elif base_group_track.name == ReferenceTrack.TRACK_NAME:
             return ReferenceTrack(base_group_track)
         elif VocalsTrack.TRACK_NAME == base_group_track.name.strip():
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/routing/RoutingDisplayNameDescriptor.py` & `protocol0-1.0.15/protocol0/domain/lom/track/routing/RoutingDisplayNameDescriptor.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/routing/RoutingTrackDescriptor.py` & `protocol0-1.0.15/protocol0/domain/lom/track/routing/RoutingTrackDescriptor.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/routing/TrackInputRouting.py` & `protocol0-1.0.15/protocol0/domain/lom/track/routing/TrackInputRouting.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/routing/TrackOutputRouting.py` & `protocol0-1.0.15/protocol0/domain/lom/track/routing/TrackOutputRouting.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/master/MasterTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/master/MasterTrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import partial
 
 from typing import Any
 
 from protocol0.domain.lom.device.DeviceEnum import DeviceEnum
-from protocol0.domain.lom.track.simple_track.SimpleTrackSaveStartedEvent import \
-    SimpleTrackSaveStartedEvent
+from protocol0.domain.lom.track.simple_track.SimpleTrackSaveStartedEvent import (
+    SimpleTrackSaveStartedEvent,
+)
 from protocol0.domain.lom.track.simple_track.audio.SimpleAudioTrack import SimpleAudioTrack
 from protocol0.domain.shared.backend.Backend import Backend
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
 from protocol0.domain.shared.scheduler.Scheduler import Scheduler
 from protocol0.domain.shared.utils.utils import volume_to_db
 
 
@@ -16,15 +17,17 @@
     IS_ACTIVE = False
 
     def __init__(self, *a, **k):
         # type: (Any, Any) -> None
         super(MasterTrack, self).__init__(*a, **k)
 
         self.devices.register_observer(self)
-        DomainEventBus.subscribe(SimpleTrackSaveStartedEvent, self._on_simple_track_save_started_event)
+        DomainEventBus.subscribe(
+            SimpleTrackSaveStartedEvent, self._on_simple_track_save_started_event
+        )
 
     def _on_simple_track_save_started_event(self, _):
         # type: (SimpleTrackSaveStartedEvent) -> None
         """youlean makes saving a track 10s + long"""
         youlean = self.devices.get_one_from_enum(DeviceEnum.YOULEAN)
 
         if youlean is not None:
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/SimpleAudioTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/SimpleAudioTrack.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/SimpleReturnTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/SimpleReturnTrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,9 @@
 
 class SimpleReturnTrack(SimpleAudioTrack):
     IS_ACTIVE = False
 
     def __init__(self, *a, **k):
         # type: (Any, Any) -> None
         super(SimpleReturnTrack, self).__init__(*a, **k)
-        Scheduler.defer(
-            partial(setattr, self.appearance, "color", TrackColorEnum.RETURN.value)
-        )
+        Scheduler.defer(partial(setattr, self.appearance, "color", TrackColorEnum.RETURN.value))
         self.appearance.disconnect()
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/audio/special/ReferenceTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/audio/special/ReferenceTrack.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 
 class ReferenceTrack(AbstractGroupTrack):
     TRACK_NAME = "Reference"
 
     def __init__(self, *a, **k):
         # type: (Any, Any) -> None
         super(ReferenceTrack, self).__init__(*a, **k)
-        mastering_rack = Song.master_track().devices.get_one_from_enum(
-            DeviceEnum.MASTERING_RACK)
+        mastering_rack = Song.master_track().devices.get_one_from_enum(DeviceEnum.MASTERING_RACK)
         self._mastering_rack_enabled = mastering_rack is not None and mastering_rack.is_enabled
 
     def toggle(self):
         # type: () -> None
-        mastering_rack = Song.master_track().devices.get_one_from_enum(
-            DeviceEnum.MASTERING_RACK)
+        mastering_rack = Song.master_track().devices.get_one_from_enum(DeviceEnum.MASTERING_RACK)
 
         if self.muted:
             self.muted = False
             self.solo = True
             if mastering_rack is not None:
                 self._mastering_rack_enabled = mastering_rack.is_enabled
                 mastering_rack.is_enabled = False
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/AudioToMidiClipMapping.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/AudioToMidiClipMapping.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/midi/SimpleMidiTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/midi/SimpleMidiTrack.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/midi/special/UsamoTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/midi/special/UsamoTrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any
 
 from protocol0.domain.lom.device.DeviceEnum import DeviceEnum
 from protocol0.domain.lom.track.group_track.ext_track.ExtArmedEvent import (
     ExtArmedEvent,
 )
-from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import \
-    ExternalSynthTrack
+from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import ExternalSynthTrack
 from protocol0.domain.lom.track.simple_track.SimpleTrackArmedEvent import SimpleTrackArmedEvent
 from protocol0.domain.lom.track.simple_track.midi.SimpleMidiTrack import SimpleMidiTrack
 from protocol0.domain.shared.errors.Protocol0Error import Protocol0Error
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
 from protocol0.domain.track_recorder.external_synth.ExtAudioRecordingStartedEvent import (
     ExtAudioRecordingStartedEvent,
 )
@@ -28,17 +27,15 @@
         # type: (Any, Any) -> None
         super(UsamoTrack, self).__init__(*a, **k)
         self._usamo_device = self.devices.get_one_from_enum(DeviceEnum.USAMO)
         if self._usamo_device is None:
             raise Protocol0Error("Cannot find usamo device on usamo track")
 
         DomainEventBus.subscribe(SimpleTrackArmedEvent, self._on_simple_track_armed_event)
-        DomainEventBus.subscribe(
-            ExtArmedEvent, self._on_external_synth_track_armed_event
-        )
+        DomainEventBus.subscribe(ExtArmedEvent, self._on_external_synth_track_armed_event)
         DomainEventBus.subscribe(
             ExtAudioRecordingStartedEvent,
             self._on_external_synth_audio_recording_started_event,
         )
 
     def _activate(self):
         # type: () -> None
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleMatchingTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/group_track/ext_track/ExtMatchingTrack.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,56 @@
-from typing import Any, Optional
+from typing import cast, Optional
 
 from protocol0.domain.lom.clip.ClipColorEnum import ClipColorEnum
 from protocol0.domain.lom.clip.ClipInfo import ClipInfo
 from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackClipColorManager import (
     MatchingTrackClipColorManager,
 )
 from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackInterface import (
     MatchingTrackInterface,
 )
-from protocol0.domain.lom.track.group_track.matching_track.utils import assert_valid_track_name, \
-    ensure_clips_looped
-from protocol0.shared.Song import Song
+from protocol0.domain.lom.track.simple_track.audio.SimpleAudioTrack import SimpleAudioTrack
 from protocol0.shared.sequence.Sequence import Sequence
 
 
-class SimpleMatchingTrack(MatchingTrackInterface):
-    def __init__(self, *a, **k):
-        # type: (Any, Any) -> None
-        super(SimpleMatchingTrack, self).__init__(*a, **k)
-        # clean the mixer if necessary (e.g. when loading back a midi track for the 1st time)
-        self._base_track.reset_mixer()
+class ExtMatchingTrack(MatchingTrackInterface):
+    def __init__(self, base_track):
+        # type: (SimpleAudioTrack) -> None
+        super(ExtMatchingTrack, self).__init__(base_track)
+        self._midi_sub_track = cast(SimpleAudioTrack, base_track.sub_tracks[0])
+        self._audio_sub_track = cast(SimpleAudioTrack, base_track.sub_tracks[1])
+        # in this setup the mapping is shared between 3 audio tracks
+        self._audio_track.clip_mapping.update(self._audio_sub_track.clip_mapping)
+        self._audio_sub_track.clip_mapping = self._audio_track.clip_mapping
 
     @property
     def clip_color_manager(self):
         # type: () -> Optional[MatchingTrackClipColorManager]
-        return MatchingTrackClipColorManager(self.router, self._base_track, self._audio_track)
-
-    def init_clips(self):
-        # type: () -> None
-        for clip in self._base_track.clips:
-            clip.previous_hash = clip.get_hash(self._base_track.devices.parameters)
+        return MatchingTrackClipColorManager(
+            self.router, self._midi_sub_track, self._audio_track, self._audio_sub_track
+        )
 
     def bounce(self):
         # type: () -> Optional[Sequence]
+        assert len(list(self._base_track.devices)) == 0, "Please move devices to audio track"
         assert self._base_track.devices.mixer_device.is_default, "Mixer was changed"
-        assert_valid_track_name(self._base_track.name)
-
-        ensure_clips_looped(self._base_track.clips)
 
-        # maintain hash / path link on hash change (update)
-        for clip in self._base_track.clips:
-            clip_hash = clip.get_hash(self._base_track.devices.parameters)
-            if clip.previous_hash == clip_hash:
-                continue
-
-            self._audio_track.clip_mapping.register_hash_equivalence(
-                clip.previous_hash, clip_hash
-            )
-            clip.previous_hash = clip_hash
-
-        bounced_clips = [c for c in self._base_track.clips if c.color == ClipColorEnum.DISABLED.value]
-        for clip in bounced_clips:
+        bounced_clips = [
+            (mc, ac)
+            for (mc, ac) in zip(self._midi_sub_track.clips, self._audio_sub_track.clips)
+            if mc.color == ClipColorEnum.DISABLED.value and ac.color == ClipColorEnum.DISABLED.value
+        ]
+        bounced_clips_flat = [c for clips in bounced_clips for c in clips]
+        for clip in bounced_clips_flat:
             assert ClipInfo(clip, self._base_track.devices.parameters).already_bounced_to(
                 self._audio_track
-            ), "clip disabled but not bounced: %s" % clip
+            ), ("clip disabled but not bounced: %s" % clip)
 
         seq = Sequence()
+
+        seq.add(self._base_track.abstract_track.arm_state.unarm)
         seq.add(self._base_track.save)
-        seq.add([c.delete for c in bounced_clips])
-        seq.add(self._base_track.flatten)
-        seq.add(lambda: Song.selected_track().delete())
+        seq.add([c.delete for c in bounced_clips_flat])
+        seq.add(self._audio_sub_track.flatten)
+        seq.add(self._base_track.delete)
 
         return seq.done()
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleMatchingTrackCreator.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleMatchingTrackCreator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from functools import partial
 
 from typing import Dict, TYPE_CHECKING
 
-from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackCreatorInterface import \
-    MatchingTrackCreatorInterface
+from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackCreatorInterface import (
+    MatchingTrackCreatorInterface,
+)
 from protocol0.domain.shared.backend.Backend import Backend
-from protocol0.domain.lom.track.group_track.matching_track.utils import assert_valid_track_name, \
-    ensure_clips_looped
+from protocol0.domain.lom.track.group_track.matching_track.utils import (
+    assert_valid_track_name,
+    ensure_clips_looped,
+)
 from protocol0.shared.Song import Song
 from protocol0.shared.sequence.Sequence import Sequence
 
 if TYPE_CHECKING:
     from protocol0.domain.lom.track.simple_track.audio.SimpleAudioTrack import SimpleAudioTrack
 
 
@@ -35,8 +38,8 @@
         return seq.done()
 
     def _post_bounce(self, mixer_data):
         # type: (Dict) -> None
         from protocol0.domain.lom.track.simple_track.audio.SimpleAudioTrack import SimpleAudioTrack
 
         flattened_track = Song.selected_track(SimpleAudioTrack)
-        flattened_track.devices.mixer_device.update_from_dict(mixer_data)
+        flattened_track.devices.mixer_device.update_from_dict(mixer_data)
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrack.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrack.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackArmState.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackArmState.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackClipColorManager.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackClipColorManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from protocol0.domain.lom.clip.ClipInfo import ClipInfo
 from protocol0.domain.lom.device.SimpleTrackDevices import SimpleTrackDevices
 
 if TYPE_CHECKING:
     from protocol0.domain.lom.track.simple_track.SimpleTrackClips import SimpleTrackClips
 
 
-
-
 class SimpleTrackClipColorManager(object):
     def __init__(self, clips, track_devices, track_color):
         # type: (SimpleTrackClips, SimpleTrackDevices, int) -> None
         self._clips = clips
         self._track_devices = track_devices
         self._track_color = track_color
 
@@ -30,17 +28,15 @@
         for clip in self._clips:
             clip.color = self._track_color
 
     def _set_colors(self):
         # type: () -> None
         color_index = 0
 
-        clip_infos = ClipInfo.create_from_clips(
-            list(self._clips), self._track_devices.parameters
-        )
+        clip_infos = ClipInfo.create_from_clips(list(self._clips), self._track_devices.parameters)
 
         for clip_info in clip_infos:
             clips = clip_info.get_clips(list(self._clips))
             for clip in clips:
                 clip.color = color_index
 
             color_index += 1
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackClips.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackClips.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, TYPE_CHECKING, Iterator
 
 from protocol0.domain.lom.clip.Clip import Clip
 from protocol0.domain.lom.device.SimpleTrackDevices import SimpleTrackDevices
-from protocol0.domain.lom.track.simple_track.SimpleTrackClipColorManager import \
-    SimpleTrackClipColorManager
+from protocol0.domain.lom.track.simple_track.SimpleTrackClipColorManager import (
+    SimpleTrackClipColorManager,
+)
 
 if TYPE_CHECKING:
     from protocol0.domain.lom.track.simple_track.SimpleTrackClipSlots import SimpleTrackClipSlots
 
 
 class SimpleTrackClips(object):
     def __init__(self, clip_slots, track_devices, track_color):
@@ -19,9 +20,11 @@
         # type: () -> Iterator[Clip]
         return iter(self._clips)
 
     @property
     def _clips(self):
         # type: () -> List[Clip]
         return [
-            clip_slot.clip for clip_slot in list(self._clip_slots) if clip_slot.has_clip and clip_slot.clip
+            clip_slot.clip
+            for clip_slot in list(self._clip_slots)
+            if clip_slot.has_clip and clip_slot.clip
         ]
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackClipSlots.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackClipSlots.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def build(self):
         # type: () -> None
         """create new ClipSlot objects and keep existing ones"""
         live_cs_to_cs = {cs._clip_slot: cs for cs in self.clip_slots}
 
         new_clip_slots = []  # type: List[ClipSlot]
-        for (index, live_clip_slot) in enumerate(list(self._live_track.clip_slots)):
+        for index, live_clip_slot in enumerate(list(self._live_track.clip_slots)):
             if live_clip_slot in live_cs_to_cs:
                 clip_slot = live_cs_to_cs[live_clip_slot]
                 # reindexing is necessary
                 clip_slot.index = index
                 if clip_slot.clip is not None:
                     clip_slot.clip.index = index
                 new_clip_slots.append(clip_slot)
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackMonitoringState.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackMonitoringState.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/simple_track/SimpleTrackService.py` & `protocol0-1.0.15/protocol0/domain/lom/track/simple_track/SimpleTrackService.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from protocol0.domain.lom.track.simple_track.SimpleTrackFlattenedEvent import \
-    SimpleTrackFlattenedEvent
+from protocol0.domain.lom.track.simple_track.SimpleTrackFlattenedEvent import (
+    SimpleTrackFlattenedEvent,
+)
 from protocol0.domain.lom.track.simple_track.audio.SimpleAudioTrack import SimpleAudioTrack
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
 from protocol0.shared.Song import Song
 
 
 class SimpleTrackService(object):
     def __init__(self):
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/TrackAutomationService.py` & `protocol0-1.0.15/protocol0/domain/lom/track/TrackAutomationService.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,8 +145,9 @@
 
         if not len(device_parameters):
             Backend.client().show_warning("No automation")
         else:
             parameters_name = ["%s: %s" % (d.name, p.name) for d, p in set(device_parameters)]
 
             Backend.client().show_info(
-                "Automated parameters: \n\n  - {}".format("\n  - ".join(parameters_name)))
+                "Automated parameters: \n\n  - {}".format("\n  - ".join(parameters_name))
+            )
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/TrackFactory.py` & `protocol0-1.0.15/protocol0/domain/lom/track/TrackFactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,23 +77,27 @@
     def add_sample_track(self, category, sample_sub_category):
         # type: (SampleCategoryEnum, str) -> Sequence
         sample_group_track = Song.drums_track()
         if sample_group_track is None:
             raise Protocol0Warning("Sample group track doesn't exist")
 
         if sample_sub_category.lower() not in category.subcategories:
-            raise Protocol0Warning("Cannot find %s sample category for '%s'" % (category, sample_sub_category))
+            raise Protocol0Warning(
+                "Cannot find %s sample category for '%s'" % (category, sample_sub_category)
+            )
 
         sample_category = SampleCategory(category, sample_sub_category)
 
         sample_group_track.base_track.is_folded = False
 
         seq = Sequence()
         seq.add(
-            partial(self._track_crud_component.create_midi_track, sample_category.create_track_index)
+            partial(
+                self._track_crud_component.create_midi_track, sample_category.create_track_index
+            )
         )
         seq.add(lambda: setattr(Song.selected_track(), "volume", -15))
         seq.add(lambda: setattr(Song.selected_track(), "color", sample_category.color))
 
         # not creating clip here
         seq.add(partial(self._drum_rack_service.load_category_drum_rack, sample_category))
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/TrackMapperService.py` & `protocol0-1.0.15/protocol0/domain/lom/track/TrackMapperService.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,18 @@
 
     def _replace_simple_track(self, previous_simple_track, new_simple_track):
         # type: (SimpleTrack, SimpleTrack) -> None
         """disconnecting and removing from SimpleTrack group track and abstract_group_track"""
         new_simple_track._index = previous_simple_track._index
         previous_simple_track.disconnect()
 
-        if previous_simple_track.group_track is not None and previous_simple_track.group_track.abstract_group_track is not None:
+        if (
+            previous_simple_track.group_track is not None
+            and previous_simple_track.group_track.abstract_group_track is not None
+        ):
             previous_simple_track.group_track.abstract_group_track.add_or_replace_sub_track(
                 new_simple_track, previous_simple_track
             )
 
         if previous_simple_track.abstract_group_track is not None:
             previous_simple_track.abstract_group_track.add_or_replace_sub_track(
                 new_simple_track, previous_simple_track
@@ -181,16 +184,15 @@
             previous_abstract_group_track = track.abstract_group_track
             abstract_group_track = self._track_factory.create_abstract_group_track(track)
 
             if isinstance(previous_abstract_group_track, ExternalSynthTrack) and isinstance(
                 abstract_group_track, NormalGroupTrack
             ):
                 Backend.client().show_warning(
-                    "%s changed into %s"
-                    % (previous_abstract_group_track, abstract_group_track)
+                    "%s changed into %s" % (previous_abstract_group_track, abstract_group_track)
                 )
 
             if (
                 previous_abstract_group_track
                 and previous_abstract_group_track != abstract_group_track
             ):
                 previous_abstract_group_track.disconnect()
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/track/TrackService.py` & `protocol0-1.0.15/protocol0/domain/lom/track/TrackService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/external_synth_track/ExternalSynthTrackValidator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/external_synth_track/SimpleAudioExtTrackValidator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/external_synth_track/SimpleMidiExtTrackValidator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from protocol0.domain.lom.device.DeviceEnum import DeviceEnum
 from protocol0.domain.lom.track.group_track.ext_track.SimpleMidiExtTrack import SimpleMidiExtTrack
 from protocol0.domain.lom.track.routing.InputRoutingChannelEnum import InputRoutingChannelEnum
 from protocol0.domain.lom.track.routing.InputRoutingTypeEnum import InputRoutingTypeEnum
 from protocol0.domain.lom.track.routing.OutputRoutingTypeEnum import OutputRoutingTypeEnum
 from protocol0.domain.lom.validation.sub_validators.AggregateValidator import AggregateValidator
-from protocol0.domain.lom.validation.sub_validators.PropertyValueValidator import \
-    PropertyValueValidator
-from protocol0.domain.lom.validation.sub_validators.SimpleTrackHasDeviceValidator import \
-    SimpleTrackHasDeviceValidator
+from protocol0.domain.lom.validation.sub_validators.PropertyValueValidator import (
+    PropertyValueValidator,
+)
+from protocol0.domain.lom.validation.sub_validators.SimpleTrackHasDeviceValidator import (
+    SimpleTrackHasDeviceValidator,
+)
 from protocol0.domain.shared.BrowserServiceInterface import BrowserServiceInterface
 
 
 class SimpleMidiExtTrackValidator(AggregateValidator):
     def __init__(self, track, browser_service):
         # type: (SimpleMidiExtTrack, BrowserServiceInterface) -> None
         self._track = track
 
         validators = [
             PropertyValueValidator(track, "volume", 0, name="midi track volume"),
             PropertyValueValidator(track, "muted", True, name="midi track muted"),
-            SimpleTrackHasDeviceValidator(
-                track, DeviceEnum.EXTERNAL_AUDIO_EFFECT, browser_service
-            ),
+            SimpleTrackHasDeviceValidator(track, DeviceEnum.EXTERNAL_AUDIO_EFFECT, browser_service),
             PropertyValueValidator(
                 track.input_routing,
                 "type",
                 InputRoutingTypeEnum.ALL_INS,
                 "midi track input type",
             ),
             PropertyValueValidator(
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/SceneValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/SceneValidator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/object_validators/SimpleAudioTrackValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/object_validators/SimpleAudioTrackValidator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/AggregateValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/AggregateValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 class AggregateValidator(ValidatorInterface):
     def __init__(self, validators):
         # type: (List[ValidatorInterface]) -> None
         self._validators = validators
 
     def get_error_message(self):
         # type: () -> Optional[str]
-        error_messages = list(filter(
-            None, [validator.get_error_message() for validator in self._validators]
-        ))
+        error_messages = list(
+            filter(None, [validator.get_error_message() for validator in self._validators])
+        )
         if len(error_messages) == 0:
             return None
         else:
             return "\n".join(error_messages)
 
     def is_valid(self):
         # type: () -> bool
```

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/CallbackValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/CallbackValidator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/DeviceParameterValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/DeviceParameterValidator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/PropertyValueValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/PropertyValueValidator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/sub_validators/SimpleTrackHasDeviceValidator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/ValidatorFactory.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/ValidatorFactory.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/ValidatorInterface.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/ValidatorInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/lom/validation/ValidatorService.py` & `protocol0-1.0.15/protocol0/domain/lom/validation/ValidatorService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/ApplicationView.py` & `protocol0-1.0.15/protocol0/domain/shared/ApplicationView.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/backend/Backend.py` & `protocol0-1.0.15/protocol0/domain/shared/backend/Backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import logging
 from functools import wraps
 
-from p0_backend_client import ApiClient
 from typing import Optional, Callable, Any
 
+from protocol0.domain.shared.backend.p0_backend_client.api.default_api import P0BackendClient
 from protocol0.shared.logging.Logger import Logger
 from protocol0.shared.types import Func
 
 
 def show_and_log(backend_client_func, log_func):
     # type: (Func, Func) -> Func
     @wraps(backend_client_func)
@@ -22,19 +23,20 @@
     """Backend API facade"""
 
     _INSTANCE = None  # type: Optional[Backend]
 
     def __init__(self, send_midi):
         # type: (Callable) -> None
         Backend._INSTANCE = self
-        self._client = ApiClient(send_midi)
+        logging.info(P0BackendClient)
+        self._client = P0BackendClient(send_midi)
 
         # wrap backend notification to also log
         self._client.show_info = show_and_log(self._client.show_info, Logger.info)
         self._client.show_success = show_and_log(self._client.show_success, Logger.info)
         self._client.show_warning = show_and_log(self._client.show_warning, Logger.warning)
         self._client.show_error = show_and_log(self._client.show_error, Logger.warning)
 
     @classmethod
     def client(cls):
-        # type: () -> ApiClient
+        # type: () -> P0BackendClient
         return cls._INSTANCE._client
```

### Comparing `protocol0-1.0.13/protocol0/domain/shared/BrowserServiceInterface.py` & `protocol0-1.0.15/protocol0/domain/shared/BrowserServiceInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/errors/error_handler.py` & `protocol0-1.0.15/protocol0/domain/shared/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/event/DomainEventBus.py` & `protocol0-1.0.15/protocol0/domain/shared/event/DomainEventBus.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/LiveObject.py` & `protocol0-1.0.15/protocol0/domain/shared/LiveObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing_extensions import Protocol
 from typing import Any
 
 
 def liveobj_valid(obj):
     # type: (Any) -> bool
-    u"""
+    """
     Check whether obj represents a valid Live API obj.
 
     This will return False both if obj represents a lost weakref or is None.
     It's important that Live API objects are not checked using "is None", since this
     would treat lost weakrefs as valid.
     """
     return obj != None  # noqa
```

### Comparing `protocol0-1.0.13/protocol0/domain/shared/LiveObjectMapping.py` & `protocol0-1.0.15/protocol0/domain/shared/LiveObjectMapping.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/scheduler/Scheduler.py` & `protocol0-1.0.15/protocol0/domain/shared/scheduler/Scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     def wait_beats(cls, beats, callback, execute_on_song_stop=False):
         # type: (float, Callable, bool) -> None
         cls._INSTANCE._beat_scheduler.wait_beats(beats, callback, execute_on_song_stop)
 
     @classmethod
     def wait_bars(cls, bars, callback, execute_on_song_stop=False):
         # type: (float, Callable, bool) -> None
-        cls._INSTANCE._beat_scheduler.wait_beats(bars * Song.signature_numerator(), callback, execute_on_song_stop)
+        cls._INSTANCE._beat_scheduler.wait_beats(
+            bars * Song.signature_numerator(), callback, execute_on_song_stop
+        )
 
     @classmethod
     def wait(cls, tick_count, callback, unique=False):
         # type: (int, Callable, bool) -> TickSchedulerEventInterface
         """
         tick_count ~= 17 ms
         unique: accept only one callback of a type. the next callback will cancel the
```

### Comparing `protocol0-1.0.13/protocol0/domain/shared/scheduler/TickSchedulerInterface.py` & `protocol0-1.0.15/protocol0/domain/shared/scheduler/TickSchedulerInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/utils/concurrency.py` & `protocol0-1.0.15/protocol0/domain/shared/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/utils/debug.py` & `protocol0-1.0.15/protocol0/domain/shared/utils/debug.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     call_frame = inspect.currentframe()
     for _ in range(frame_count):
         next_frame = call_frame.f_back
         if not next_frame:
             break
         call_frame = next_frame
     try:
-        (filename, line, method_name, _, _) = inspect.getframeinfo(call_frame)
+        (filename, line, method_name, _, _) = inspect.getframeinfo(call_frame)  # type: ignore[arg-type]
     except IndexError:
         return None
     filename = filename.replace(Config.PROJECT_ROOT + "\\", "").replace(
         Config.REMOTE_SCRIPTS_ROOT + "\\", ""
     )
     class_name = filename.replace(".py", "").split("\\")[-1]
```

### Comparing `protocol0-1.0.13/protocol0/domain/shared/utils/forward_to.py` & `protocol0-1.0.15/protocol0/domain/shared/utils/forward_to.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/utils/func.py` & `protocol0-1.0.15/protocol0/domain/shared/utils/func.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,14 @@
     if class_ is None:
         raise Protocol0Error("Cannot get class_name from func")
 
     class_name = class_.__name__
     if class_name and all(word not in class_name for word in ["function", "None"]):
         return class_name
 
-
-
     try:
         if sys.version_info.major == 2:
             from qualname import qualname
 
             func_qualname = qualname(func)
         else:
             func_qualname = func.__qualname__
```

### Comparing `protocol0-1.0.13/protocol0/domain/shared/utils/timing.py` & `protocol0-1.0.15/protocol0/domain/shared/utils/timing.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,32 +106,32 @@
 
     return wrap
 
 
 def accelerate(func):
     # type: (Func) -> Func
     """
-        Function used to soft accelerate parameter scrolling as done in the hardware
-        Function that will transmit the number of times it was called during the last second
-        The count is given in the factor keyword argument
-        Useful for implementing input acceleration
+    Function used to soft accelerate parameter scrolling as done in the hardware
+    Function that will transmit the number of times it was called during the last second
+    The count is given in the factor keyword argument
+    Useful for implementing input acceleration
     """
     # in ms : the duration considered for increasing the acceleration factor
     ACCELERATION_ACTIVATION_DURATION = 700
     # above this is too fast
     MAX_ACCELERATION = 20
     # number of calls allowed before acceleration starts
     FINE_TUNING_RANGE = 2
 
     @wraps(func)
     def decorate(*a, **k):
         # type: (Any, Any) -> None
         object_source = a[0] if inspect.ismethod(func) else decorate
 
-        last_calls = decorate.last_calls[object_source]    # type: ignore[attr-defined]
+        last_calls = decorate.last_calls[object_source]  # type: ignore[attr-defined]
         last_calls.append(time.time())
 
         duration_second = float(ACCELERATION_ACTIVATION_DURATION) / 1000
         last_calls = list(filter(lambda t: t >= time.time() - duration_second, last_calls))
         decorate.last_calls[object_source] = last_calls  # type: ignore[attr-defined]
 
         acceleration = len(last_calls) - FINE_TUNING_RANGE + 1
```

### Comparing `protocol0-1.0.13/protocol0/domain/shared/utils/utils.py` & `protocol0-1.0.15/protocol0/domain/shared/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,8 +136,8 @@
 
 
 def float_seq(start, end, step):
     # type: (int, int, float) -> Iterable
     assert step != 0
     sample_count = int(abs(end - start) / step)
 
-    return itertools.islice(itertools.count(start, step), sample_count)  # type: ignore
+    return itertools.islice(itertools.count(start, step), sample_count)
```

### Comparing `protocol0-1.0.13/protocol0/domain/shared/ValueScroller.py` & `protocol0-1.0.15/protocol0/domain/shared/ValueScroller.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/shared/ValueToggler.py` & `protocol0-1.0.15/protocol0/domain/shared/ValueToggler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/AbstractRecorderFactory.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/AbstractRecorderFactory.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/BaseRecorder.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/BaseRecorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,15 @@
         seq = Sequence()
         seq.add([clip_slot.prepare_for_record for clip_slot in self.config.clip_slots])
         return seq.done()
 
     def _arm_track(self):
         # type: () -> Sequence
         seq = Sequence()
-        if (
-            not Song.current_track().arm_state.is_armed
-            and len(list(Song.armed_tracks())) != 0
-        ):
+        if not Song.current_track().arm_state.is_armed and len(list(Song.armed_tracks())) != 0:
             options = ["Arm current track", "Record on armed track"]
             seq.select("The current track is not armed", options=options)
             seq.add(
                 lambda: self._track.arm_state.arm()
                 if seq.res == options[0]
                 else setattr(self, "_track", list(Song.armed_tracks())[0])
             )
@@ -51,19 +48,21 @@
             seq.add(self._track.arm_state.arm)
 
         return seq.done()
 
     def record(self):
         # type: () -> Sequence
         # launch the record
-        DomainEventBus.emit(RecordStartedEvent(
-            self.config.scene_index,
-            full_record=self.config.bar_length == 0,
-            has_count_in=self.config.records_midi
-        ))
+        DomainEventBus.emit(
+            RecordStartedEvent(
+                self.config.scene_index,
+                full_record=self.config.bar_length == 0,
+                has_count_in=self.config.records_midi,
+            )
+        )
         seq = Sequence()
         bar_length = cast(float, self.config.bar_length)
         if bar_length != 0:
             if not Song.is_playing():
                 seq.wait_for_event(SongStartedEvent)
             if not self.config.records_midi:
                 # play well with the tail recording
```

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/config/RecordConfig.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/config/RecordConfig.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/config/RecordProcessors.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/config/RecordProcessors.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,22 +14,20 @@
         self.record = record
         self.on_record_end = on_record_end
         self.post_record = post_record
 
     def __repr__(self):
         # type: () -> str
         # noinspection SpellCheckingInspection
-        return "RecordProcessors(\npre_record=%s,\nrecord=%s,\non_record_end=%s,\npost_record=%s" % (
-            self.pre_record,
-            self.record,
-            self.on_record_end,
-            self.post_record
+        return (
+            "RecordProcessors(\npre_record=%s,\nrecord=%s,\non_record_end=%s,\npost_record=%s"
+            % (self.pre_record, self.record, self.on_record_end, self.post_record)
         )
 
     def copy(self):
         # type: () -> RecordProcessors
         return RecordProcessors(
             pre_record=self.pre_record,
             record=self.record,
             on_record_end=self.on_record_end,
             post_record=self.post_record,
-        )
+        )
```

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/count_in/CountInOneBar.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/count_in/CountInOneBar.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/count_in/CountInShort.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/count_in/CountInShort.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/OnRecordEndClipTail.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/OnRecordEndClipTail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from functools import partial
 
 from typing import Optional
 
-from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import \
-    ExternalSynthTrack
+from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import ExternalSynthTrack
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
 from protocol0.domain.shared.scheduler.Last32thPassedEvent import Last32thPassedEvent
 from protocol0.domain.track_recorder.config.RecordConfig import RecordConfig
 from protocol0.domain.track_recorder.RecordProcessorInterface import RecordProcessorInterface
 from protocol0.domain.track_recorder.external_synth.AudioClipSilentEvent import (
     AudioClipSilentEvent,
 )
@@ -50,15 +49,14 @@
 
         if audio_clip is None:
             return None
 
         audio_clip.loop.looping = False
         track.midi_track.stop()
 
-
         def on_last_32th_passed_event(_):
             # type: (Last32thPassedEvent) -> None
             if self.is_audio_silent(track):
                 DomainEventBus.emit(AudioClipSilentEvent())
                 DomainEventBus.un_subscribe(Last32thPassedEvent, on_last_32th_passed_event)
 
         DomainEventBus.subscribe(Last32thPassedEvent, on_last_32th_passed_event)
```

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/PostRecordAudio.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/PostRecordAudio.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/PostRecordAudioFull.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import \
-    ExternalSynthTrack
+from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import ExternalSynthTrack
 from protocol0.domain.track_recorder.RecordProcessorInterface import RecordProcessorInterface
 from protocol0.domain.track_recorder.config.RecordConfig import RecordConfig
-from protocol0.domain.track_recorder.external_synth.record_audio.PostRecordAudio import \
-    PostRecordAudio
+from protocol0.domain.track_recorder.external_synth.record_audio.PostRecordAudio import (
+    PostRecordAudio,
+)
 from protocol0.shared.Song import Song
 
 
 class PostRecordAudioFull(RecordProcessorInterface):
     def process(self, track, config):
         # type: (ExternalSynthTrack, RecordConfig) -> None
         PostRecordAudio().process(track, config)
```

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/PreRecordAudio.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/PreRecordAudio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import \
-    ExternalSynthTrack
+from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import ExternalSynthTrack
 from protocol0.domain.shared.backend.Backend import Backend
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
 from protocol0.domain.track_recorder.config.RecordConfig import RecordConfig
 from protocol0.domain.track_recorder.RecordProcessorInterface import RecordProcessorInterface
-from protocol0.domain.track_recorder.external_synth.ExtAudioRecordingStartedEvent import \
-    ExtAudioRecordingStartedEvent
+from protocol0.domain.track_recorder.external_synth.ExtAudioRecordingStartedEvent import (
+    ExtAudioRecordingStartedEvent,
+)
 
 
 class PreRecordAudio(RecordProcessorInterface):
     def process(self, track, config):
         # type: (ExternalSynthTrack, RecordConfig) -> None
         track.monitoring_state.monitor_midi()
         midi_clip = track.midi_track.clip_slots[config.scene_index].clip
```

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/PreRecordAudioMulti.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from protocol0.domain.shared.backend.Backend import Backend
 from protocol0.domain.shared.event.DomainEventBus import DomainEventBus
 from protocol0.domain.track_recorder.config.RecordConfig import RecordConfig
 from protocol0.domain.track_recorder.RecordProcessorInterface import RecordProcessorInterface
 from protocol0.domain.track_recorder.external_synth.ExtAudioRecordingStartedEvent import (
     ExtAudioRecordingStartedEvent,
 )
-from protocol0.domain.track_recorder.external_synth.record_audio.PreRecordAudio import \
-    PreRecordAudio
+from protocol0.domain.track_recorder.external_synth.record_audio.PreRecordAudio import (
+    PreRecordAudio,
+)
 
 
 class PreRecordAudioMulti(RecordProcessorInterface):
     def process(self, track, config):
         # type: (ExternalSynthTrack, RecordConfig) -> None
         """
         Alerting when a midi clip does not have the same bar length as its scene (except for the last one)
```

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_audio/record_multi/RecordAudioMulti.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from functools import partial
 
 from typing import Optional
 
 from protocol0.domain.lom.scene.SceneLastBarPassedEvent import SceneLastBarPassedEvent
-from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import \
-    ExternalSynthTrack
+from protocol0.domain.lom.track.group_track.ext_track.ExternalSynthTrack import ExternalSynthTrack
 from protocol0.domain.shared.scheduler.BarChangedEvent import BarChangedEvent
 from protocol0.domain.track_recorder.config.RecordConfig import RecordConfig
 from protocol0.domain.track_recorder.RecordProcessorInterface import RecordProcessorInterface
 from protocol0.shared.sequence.Sequence import Sequence
 
 
 class RecordAudioMulti(RecordProcessorInterface):
```

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/record_midi/PostRecordMidi.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/record_midi/PostRecordMidi.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/external_synth/TrackRecorderExternalSynthFactory.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/recording_bar_length/RecordingBarLengthEnum.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/recording_bar_length/RecordingBarLengthScroller.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/RecordProcessorInterface.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/RecordProcessorInterface.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/RecordService.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/RecordService.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,14 @@
             seq.add(partial(processors.pre_record.process, track, config))
         seq.add(partial(record_type.get_count_in().launch, self._playback_component, track))
         seq.add(partial(DomainEventBus.subscribe, SongStoppedEvent, self._on_song_stopped_event))
 
         if not config.records_midi:
             seq.wait_ms(50)  # so that the record doesn't start before the clip slot is ready
 
-
         # RECORD
         if processors.record is not None:
             seq.add(partial(processors.record.process, track, config))
         else:
             seq.add(self._recorder.record)
 
         if processors.on_record_end is not None:
```

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/RecordTypeEnum.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/RecordTypeEnum.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/simple/PostRecordSimple.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/simple/PostRecordSimple.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/domain/track_recorder/simple/RecorderSimpleFactory.py` & `protocol0-1.0.15/protocol0/domain/track_recorder/simple/RecorderSimpleFactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def get_record_config(self, track, record_type, recording_bar_length):
         # type: (SimpleTrack, RecordTypeEnum, int) -> RecordConfig
         return RecordConfig(
             record_name=record_type.value,
             tracks=[track],
             scene_index=self._get_recording_scene_index(track),
             bar_length=self._get_recording_bar_length(record_type, recording_bar_length),
-            records_midi=True
+            records_midi=True,
         )
 
     def _get_recording_scene_index(self, track):
         # type: (SimpleTrack) -> Optional[int]
         for i in range(Song.selected_scene().index, len(Song.scenes())):
             if not track.clip_slots[i].clip:
                 return i
```

### Comparing `protocol0-1.0.13/protocol0/infra/interface/BrowserLoaderService.py` & `protocol0-1.0.15/protocol0/infra/interface/BrowserLoaderService.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,15 @@
         # type: (str) -> None
         """Loads items from the user library category"""
         self._do_load_item(self._get_item_for_category("user_library", name), "from User Library")
 
     def get_sample(self, sample_name):
         # type: (str) -> Live.Browser.BrowserItem
         self._cache_category("samples")
-        return self._cached_browser_items["samples"].get(
-            str(sample_name.decode("utf-8")), None
-        )
+        return self._cached_browser_items["samples"].get(sample_name, None)
 
     def _do_load_item(self, item, header="Device"):
         # type: (Live.Browser.BrowserItem, str) -> None
         """Handles loading an item and displaying load info in status bar."""
         # NB : activating this will hotswap drum rack pads if a drum rack is selected
         # ApplicationView.toggle_browse()
         if item and item.is_loadable:
```

### Comparing `protocol0-1.0.13/protocol0/infra/interface/BrowserService.py` & `protocol0-1.0.15/protocol0/infra/interface/BrowserService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/infra/interface/session/SessionService.py` & `protocol0-1.0.15/protocol0/infra/interface/session/SessionService.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,11 +55,8 @@
         if self._session:
             self._session.set_show_highlight(False)
             self._session.disconnect()
 
     @property
     def _session_track_offset(self):
         # type: () -> int
-        try:
-            pass
-        except ValueError:
-            return self._session.track_offset() if self._session else 0
+        return self._session.track_offset() if self._session else 0
```

### Comparing `protocol0-1.0.13/protocol0/infra/logging/LoggerService.py` & `protocol0-1.0.15/protocol0/infra/logging/LoggerService.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,17 +24,14 @@
                 # use str to json encode classes
                 message = json.dumps(message, indent=4, default=str)
             except (TypeError, UnicodeEncodeError) as e:
                 from protocol0.shared.logging.Logger import Logger
 
                 Logger.warning(e)
 
-        if sys.version_info.major == 2 and not isinstance(message, basestring):
-            message = str(message)
-
         level = level or LogLevelEnum.INFO
         if level.value < Config.LOG_LEVEL.value:
             return
         message = "%s: %s" % (level.name.lower(), smart_string(message))
         if not isinstance(debug, bool):
             raise Protocol0Error("logger: parameter mismatch")
         if debug:
@@ -46,11 +43,11 @@
                     message,
                     frame_info.filename,
                     frame_info.line,
                     frame_info.method_name,
                 )
         for line in message.splitlines():
             if sys.version_info.major == 2:
-                line.decode("utf-8").encode("ascii", "replace")
+                line.encode("ascii", "replace")
 
             line = "P0 - %s" % line
             logging.info(line)
```

### Comparing `protocol0-1.0.13/protocol0/infra/midi/MidiService.py` & `protocol0-1.0.15/protocol0/infra/midi/MidiService.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/infra/persistence/SongDataService.py` & `protocol0-1.0.15/protocol0/infra/persistence/SongDataService.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,33 +13,30 @@
         # type: (Callable) -> None
         self.get_value = get_value
         self.saved_value = None
 
 
 class SongDataService(object):
     """Service handling data storage in the set"""
+
     _DEBUG = False
 
     def __init__(self, get_data, set_data, scene_component):
         # type: (Callable, Callable, SceneComponent) -> None
 
         self._set_data = set_data
         self._get_data = get_data
         self._scene_component = scene_component
 
         self._elements = {
-            SongDataEnum.SELECTED_SCENE_INDEX: SongDataElement(
-                lambda: Song.selected_scene().index
-            ),
+            SongDataEnum.SELECTED_SCENE_INDEX: SongDataElement(lambda: Song.selected_scene().index),
             SongDataEnum.SELECTED_SCENE_POSITION: SongDataElement(
                 lambda: Song.selected_scene().position_scroller.current_value
             ),
-            SongDataEnum.SELECTED_TRACK_INDEX: SongDataElement(
-                lambda: Song.selected_track().index
-            ),
+            SongDataEnum.SELECTED_TRACK_INDEX: SongDataElement(lambda: Song.selected_track().index),
         }
 
         self._restore()
         DomainEventBus.subscribe(SceneFiredEvent, lambda _: self._save())
 
     def _save(self):
         # type: () -> None
@@ -59,15 +56,17 @@
     def _restore_set_state(self):
         # type: () -> None
         selected_scene_index = self._elements.get(SongDataEnum.SELECTED_SCENE_INDEX).saved_value
         if selected_scene_index is not None and selected_scene_index < len(Song.scenes()):
             selected_scene = Song.scenes()[selected_scene_index]
             self._scene_component.select_scene(selected_scene)
 
-            selected_scene_position = self._elements.get(SongDataEnum.SELECTED_SCENE_POSITION).saved_value
+            selected_scene_position = self._elements.get(
+                SongDataEnum.SELECTED_SCENE_POSITION
+            ).saved_value
             if selected_scene_position is not None:
                 selected_scene.position_scroller.set_value(selected_scene_position)
 
         selected_track_index = self._elements.get(SongDataEnum.SELECTED_TRACK_INDEX).saved_value
         if selected_track_index is not None and selected_track_index < len(
             list(Song.all_simple_tracks())
         ):
```

### Comparing `protocol0-1.0.13/protocol0/infra/persistence/TrackData.py` & `protocol0-1.0.15/protocol0/infra/persistence/TrackData.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/infra/scheduler/BeatScheduler.py` & `protocol0-1.0.15/protocol0/infra/scheduler/BeatScheduler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/infra/scheduler/BeatSchedulerEvent.py` & `protocol0-1.0.15/protocol0/infra/scheduler/BeatSchedulerEvent.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         self._execute_on_song_stop = execute_on_song_stop
 
     @property
     def should_execute(self):
         # type: () -> bool
         if Song.is_playing():
             return (
-                    BeatTime.from_song_beat_time(Song.current_beats_song_time())
-                    >= self._beats_song_execution_time
+                BeatTime.from_song_beat_time(Song.current_beats_song_time())
+                >= self._beats_song_execution_time
             )
         else:
             return self._execute_on_song_stop
 
     def execute(self):
         # type: () -> None
         self._callback()
```

### Comparing `protocol0-1.0.13/protocol0/infra/scheduler/BeatTime.py` & `protocol0-1.0.15/protocol0/infra/scheduler/BeatTime.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/infra/scheduler/TickScheduler.py` & `protocol0-1.0.15/protocol0/infra/scheduler/TickScheduler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/infra/scheduler/TickSchedulerEvent.py` & `protocol0-1.0.15/protocol0/infra/scheduler/TickSchedulerEvent.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/AbstractEnum.py` & `protocol0-1.0.15/protocol0/shared/AbstractEnum.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/Config.py` & `protocol0-1.0.15/protocol0/shared/Config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from os.path import dirname, realpath
 
 import Live
 
-from protocol0.domain.track_recorder.recording_bar_length.RecordingBarLengthEnum import \
-    RecordingBarLengthEnum
+from protocol0.domain.track_recorder.recording_bar_length.RecordingBarLengthEnum import (
+    RecordingBarLengthEnum,
+)
 from protocol0.shared.logging.LogLevelEnum import LogLevelEnum
 
 
 class Config(object):
     # DIRECTORIES
     PROJECT_ROOT = dirname(dirname(realpath(__file__)))
     REMOTE_SCRIPTS_ROOT = dirname(PROJECT_ROOT)
```

### Comparing `protocol0-1.0.13/protocol0/shared/logging/Logger.py` & `protocol0-1.0.15/protocol0/shared/logging/Logger.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/logging/StatusBar.py` & `protocol0-1.0.15/protocol0/shared/logging/StatusBar.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/module.py` & `protocol0-1.0.15/protocol0/shared/module.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,8 @@
     def __hash__(self):
         # type: () -> int
         return 0
 
     def __iter__(self):
         # type: () -> Iterator
         """Handles push2 scales"""
-        return iter([("", "")])
+        return iter([("", "")])
```

### Comparing `protocol0-1.0.13/protocol0/shared/observer/Observable.py` & `protocol0-1.0.15/protocol0/shared/observer/Observable.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/sequence/HasSequenceState.py` & `protocol0-1.0.15/protocol0/shared/sequence/HasSequenceState.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/sequence/ParallelSequence.py` & `protocol0-1.0.15/protocol0/shared/sequence/ParallelSequence.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/sequence/Sequence.py` & `protocol0-1.0.15/protocol0/shared/sequence/Sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,14 @@
 
             DomainEventBus.un_subscribe(BackendEvent, on_event)
 
             if self.state.started:
                 self.res = backend_event.data
                 self._execute_next_step()
 
-
         def cancel():
             # type: () -> None
             DomainEventBus.un_subscribe(BackendEvent, on_event)
             self._cancel()
 
         self.add(step, notify_terminated=False)
```

### Comparing `protocol0-1.0.13/protocol0/shared/sequence/SequenceState.py` & `protocol0-1.0.15/protocol0/shared/sequence/SequenceState.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/sequence/SequenceStep.py` & `protocol0-1.0.15/protocol0/shared/sequence/SequenceStep.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/sequence/SequenceTransition.py` & `protocol0-1.0.15/protocol0/shared/sequence/SequenceTransition.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/sequence/TimeoutLimit.py` & `protocol0-1.0.15/protocol0/shared/sequence/TimeoutLimit.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/shared/Song.py` & `protocol0-1.0.15/protocol0/shared/Song.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,20 +150,21 @@
             raise Protocol0Error(
                 "Couldn't find live track %s in _live_track_id_to_simple_track mapping : \n "
                 "%s" % (live_track.name, "\n".join(existing_tracks))
             )
 
         return track_mapping[live_track._live_ptr]
 
-
     @classmethod
     def optional_simple_track_from_live_track(cls, live_track):
         # type: (Live.Track.Track) -> Optional[SimpleTrack]
         try:
-            return cls._INSTANCE._track_mapper_service._live_track_id_to_simple_track[live_track._live_ptr]
+            return cls._INSTANCE._track_mapper_service._live_track_id_to_simple_track[
+                live_track._live_ptr
+            ]
         except KeyError:
             return None
 
     @classmethod
     def simple_tracks(cls, track_cls=None):
         # type: (Optional[Type[T]]) -> Iterator[T|SimpleTrack]
         from protocol0.domain.lom.track.simple_track.SimpleTrack import SimpleTrack
```

### Comparing `protocol0-1.0.13/protocol0/shared/UndoFacade.py` & `protocol0-1.0.15/protocol0/shared/UndoFacade.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
     def __init__(self, begin_undo_step, end_undo_step):
         # type: (Callable, Callable) -> None
         UndoFacade._INSTANCE = self
         self._begin_undo_step = begin_undo_step
         self._end_undo_step = end_undo_step
 
-
     @classmethod
     def begin_undo_step(cls):
         # type: () -> None
         cls._INSTANCE._end_undo_step()
 
     @classmethod
     def end_undo_step(cls):
```

### Comparing `protocol0-1.0.13/protocol0/tests/application/test_multi_encoder.py` & `protocol0-1.0.15/protocol0/tests/application/test_multi_encoder.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/clip/test_clip_playing_position.py` & `protocol0-1.0.15/protocol0/tests/domain/clip/test_clip_playing_position.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/fixtures/clip.py` & `protocol0-1.0.15/protocol0/tests/domain/fixtures/clip.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/fixtures/device.py` & `protocol0-1.0.15/protocol0/tests/domain/fixtures/device.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/fixtures/group_track.py` & `protocol0-1.0.15/protocol0/tests/domain/fixtures/group_track.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/fixtures/p0.py` & `protocol0-1.0.15/protocol0/tests/domain/fixtures/p0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+import sys
+from os.path import dirname
 from typing import Optional
+from unittest.mock import Mock
+
+sys.path.insert(0, f"{dirname(__file__)}/protocol0_stub")
 
-from protocol0 import EmptyModule
 from protocol0.application.Protocol0 import Protocol0
 from protocol0.application.control_surface.ActionGroupFactory import ActionGroupFactory
 from protocol0.domain.lom.set.AbletonSet import AbletonSet
 from protocol0.domain.lom.song.SongInitService import SongInitService
-from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackInterface import MatchingTrackInterface
+from protocol0.domain.lom.track.group_track.matching_track.MatchingTrackInterface import (
+    MatchingTrackInterface,
+)
 from protocol0.domain.lom.track.routing.RoutingTrackDescriptor import RoutingTrackDescriptor
 from protocol0.domain.lom.track.simple_track.SimpleTrack import SimpleTrack
 from protocol0.domain.shared.backend.Backend import Backend
 from protocol0.domain.shared.scheduler.Scheduler import Scheduler
 from protocol0.domain.shared.utils.func import nop
 from protocol0.infra.logging.LoggerService import LoggerService
 from protocol0.infra.scheduler.BeatScheduler import BeatScheduler
@@ -23,15 +29,15 @@
 def make_protocol0():
     # type: () -> Protocol0
     live_song = AbletonSong()
     Protocol0.song = lambda _: live_song
     wait = Scheduler.wait
     Scheduler.wait = classmethod(nop)
     monkey_patch_static()
-    p0 = Protocol0(EmptyModule(name="c_instance", is_false=False))
+    p0 = Protocol0(Mock())
     monkey_patch_p0(live_song)
     Scheduler.wait = wait
     return p0
 
 
 def monkey_patch_static():
     # hide logs
```

### Comparing `protocol0-1.0.13/protocol0/tests/domain/fixtures/simple_track.py` & `protocol0-1.0.15/protocol0/tests/domain/fixtures/simple_track.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 
     def __init__(self, track_type=TrackType.MIDI):
         # type: (str) -> None
         self._live_ptr = id(self)
         self.name = track_type
         self.devices = []  # type: List[AbletonDevice]
         mixer_device = namedtuple("mixer_device", ["sends", "volume", "panning"])
-        self.mixer_device = mixer_device([], AbletonDeviceParameter("volume"), AbletonDeviceParameter("panning"))
+        self.mixer_device = mixer_device(
+            [], AbletonDeviceParameter("volume"), AbletonDeviceParameter("panning")
+        )
         self.can_be_armed = True
         self.arm = False
         self.solo = False
         self.fold_state = False
         self.is_visible = True
         self.has_midi_input = self.is_foldable = self.fold_state = False
         self.available_input_routing_types = []
```

### Comparing `protocol0-1.0.13/protocol0/tests/domain/fixtures/song.py` & `protocol0-1.0.15/protocol0/tests/domain/fixtures/song.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/scene/test_scene_clips.py` & `protocol0-1.0.15/protocol0/tests/domain/scene/test_scene_clips.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/scene/test_scene_length.py` & `protocol0-1.0.15/protocol0/tests/domain/scene/test_scene_length.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/scene/test_scene_playing_position.py` & `protocol0-1.0.15/protocol0/tests/domain/scene/test_scene_playing_position.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/shared/event/test_domain_event_bus.py` & `protocol0-1.0.15/protocol0/tests/domain/shared/event/test_domain_event_bus.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/shared/test_live_object_mapping.py` & `protocol0-1.0.15/protocol0/tests/domain/shared/test_live_object_mapping.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/shared/utils/test_func.py` & `protocol0-1.0.15/protocol0/tests/domain/shared/utils/test_func.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/shared/utils/test_utils.py` & `protocol0-1.0.15/protocol0/tests/domain/shared/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/track/test_audio_to_midi_clip_mapping.py` & `protocol0-1.0.15/protocol0/tests/domain/track/test_audio_to_midi_clip_mapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from protocol0 import EmptyModule
+from unittest.mock import Mock
+
 from protocol0.domain.lom.track.simple_track.AudioToMidiClipMapping import AudioToMidiClipMapping
 
+
 class ClipInfoTest(object):
     def __init__(self, clip_hash):
         self.hash = clip_hash
 
 
 # noinspection PyTypeChecker
 def test_audio_to_midi_clip_mapping():
-    mapping = AudioToMidiClipMapping(EmptyModule())  # noqa
+    mapping = AudioToMidiClipMapping(Mock())
     mapping.register_file_path("path1", ClipInfoTest(1))
     mapping.register_file_path("path1_bis", ClipInfoTest(1))
     mapping.register_file_path("path2", ClipInfoTest(2))
     # modify the midi clip
     mapping.register_hash_equivalence(1, 11)
 
     assert mapping.path_matches_hash("path1", 1, False)
```

### Comparing `protocol0-1.0.13/protocol0/tests/domain/track/test_instantiation.py` & `protocol0-1.0.15/protocol0/tests/domain/track/test_instantiation.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/validation/test_aggregate_validator.py` & `protocol0-1.0.15/protocol0/tests/domain/validation/test_aggregate_validator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/validation/test_callback_validator.py` & `protocol0-1.0.15/protocol0/tests/domain/validation/test_callback_validator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/domain/validation/test_property_validator.py` & `protocol0-1.0.15/protocol0/tests/domain/validation/test_property_validator.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/infra/listeners/test_subject_slot.py` & `protocol0-1.0.15/protocol0/tests/infra/listeners/test_subject_slot.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/infra/scheduler/TickSchedulerTest.py` & `protocol0-1.0.15/protocol0/tests/infra/scheduler/TickSchedulerTest.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/infra/test_scheduler.py` & `protocol0-1.0.15/protocol0/tests/infra/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/shared/sequence/test_sanity_sequence.py` & `protocol0-1.0.15/protocol0/tests/shared/sequence/test_sanity_sequence.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/shared/sequence/test_sequence.py` & `protocol0-1.0.15/protocol0/tests/shared/sequence/test_sequence.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/shared/sequence/test_sequence_parallel.py` & `protocol0-1.0.15/protocol0/tests/shared/sequence/test_sequence_parallel.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/protocol0/tests/shared/test_container.py` & `protocol0-1.0.15/protocol0/tests/shared/test_container.py`

 * *Files identical despite different names*

### Comparing `protocol0-1.0.13/pyproject.toml` & `protocol0-1.0.15/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.6.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "protocol0"
-version = "1.0.13"
+version = "1.0.15"
 description = "Protocol0 ableton remote script"
 readme = "README.md"
 authors = ["Thibault Lebrun <thibaultlebrun@live.fr>"]
 license = "MIT"
 repository = "https://github.com/lebrunthibault/protocol0"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -34,16 +34,20 @@
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.black]
 line-length = 100
 
 [tool.mypy]
-python_version = 2.7
-exclude = ['venv', 'tests', 'vulture_whitelist.py']
+python_version = "3.7"
+exclude = [
+    'tests',
+    'vulture_whitelist.py',
+    'protocol0/domain/shared/backend/p0_backend_client'
+]
 pretty = false
 ignore_missing_imports = true
 follow_imports = 'skip'
 # cannot remove misc because of _Framework. union-attr possibly
 disable_error_code = ['misc','union-attr', 'has-type']
 show_error_codes = true
 warn_unreachable = true
@@ -63,15 +67,16 @@
 verbose = false
 exclude = [
     'venv/',
     'build/',
     'command/',
     'command_handler/',
     'push2/',
-    'BarLengthEnum.py'
+    'RecordingBarLengthEnum.py',
+    'protocol0/domain/shared/backend/p0_backend_client'
 ]
 ignore_names = [
     "subject",
     "TRACK_COLOR"
 ]
```

### Comparing `protocol0-1.0.13/README.md` & `protocol0-1.0.15/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -79,20 +79,20 @@
 > from my backend on its port to the main script. See [this repo](https://github.com/lebrunthibault/Protocol0-Midi-Surface-Script)
 > The same purpose would be achievable my external midi routing using e.g. midi ox. I like this dependency better.
 
 ## Installation
 
 `make bootstrap`
 
-### Install the script
+### Install the script in your remote scripts folder (for Live 11)
+
+- `make install_script_p0`
+- `make install_script_p0_midi` to add a midi port proxy
+
 
-- clone the repo in your remote scripts directory
-- create a python virtual env, activate it and `pip install -r .\requirements.txt`
-- Try using a configurable midi controller to match the mappings in ./application/control_surface/group. The main
-  commands are defined in ActionGroupMain
 
 ### Install the backend
 
 - clone and follow the README install section of the [backend](https://github.com/lebrunthibault/protocol0/tree/main/p0_backend).
 - You should also
```

### Comparing `protocol0-1.0.13/PKG-INFO` & `protocol0-1.0.15/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protocol0
-Version: 1.0.13
+Version: 1.0.15
 Summary: Protocol0 ableton remote script
 Home-page: https://github.com/lebrunthibault/protocol0
 License: MIT
 Keywords: remote script,ableton
 Author: Thibault Lebrun
 Author-email: thibaultlebrun@live.fr
 Requires-Python: >=3.7.3
@@ -104,20 +104,20 @@
 > from my backend on its port to the main script. See [this repo](https://github.com/lebrunthibault/Protocol0-Midi-Surface-Script)
 > The same purpose would be achievable my external midi routing using e.g. midi ox. I like this dependency better.
 
 ## Installation
 
 `make bootstrap`
 
-### Install the script
+### Install the script in your remote scripts folder (for Live 11)
+
+- `make install_script_p0`
+- `make install_script_p0_midi` to add a midi port proxy
+
 
-- clone the repo in your remote scripts directory
-- create a python virtual env, activate it and `pip install -r .\requirements.txt`
-- Try using a configurable midi controller to match the mappings in ./application/control_surface/group. The main
-  commands are defined in ActionGroupMain
 
 ### Install the backend
 
 - clone and follow the README install section of the [backend](https://github.com/lebrunthibault/protocol0/tree/main/p0_backend).
 - You should also
```

