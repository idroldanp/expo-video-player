Issue whit start in:

// Set audio mode to play even in silent mode (like the YouTube app) index.js

/*try {
            await Audio.setAudioModeAsync({
                allowsRecordingIOS: false,
                interruptionModeIOS: Audio.INTERRUPTION_MODE_IOS_DO_NOT_MIX,
                playsInSilentModeIOS: true,
                shouldDuckAndroid: true,
                interruptionModeAndroid: Audio.INTERRUPTION_MODE_ANDROID_DO_NOT_MIX,
                playThroughEarpieceAndroid: false
            });
        }
        catch (e) {
            errorCallback({
                type: ErrorSeverity.NonFatal,
                message: 'setAudioModeAsync error',
                obj: e,
            });
        }*/

And validation for scroll in seeking function

        // Seeking
        this.getSeekSliderPosition = () => {
            if (this.playbackInstance !== null &&
                this.state.playbackInstancePosition !== null &&
                this.state.playbackInstancePosition !== 0 &&
                this.state.playbackInstanceDuration !== null) {
                return (this.state.playbackInstancePosition /
                    this.state.playbackInstanceDuration);
            }
            return 0;
        };

