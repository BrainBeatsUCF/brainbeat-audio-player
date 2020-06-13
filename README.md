# brainbeats-audio-player

# NPM Installation

```
In the same directory with package.json

# Create npmrc file so the project can talk to github package
touch .npmrc

# Point the project to BrainbeatsUCF org
echo registry=https://npm.pkg.github.com/BrainBeatsUCF >> .npmrc

# Install the audio package
npm install @brainbeatsucf/brainbeats-audio-player
```

# Properties for the component
style?: React.CSSProperties
audioObjectArray: AudioObject[]

where AudioObject is:
interface AudioObject {
  title: string,
  authorName: string,
  imageUrl: string,
  audioUrl: string
}

# Usage
```
import BrainBeatsAudioPlayer from '@brainbeatsucf/brainbeats-audio-player';
import '@brainbeatsucf/brainbeats-audio-player/src/style.css';

const Player = () => {
  <AudioPlayer 
    style={{width: 400}} 
    audioObjectArray={audioObjectArray} 
  />
}
```