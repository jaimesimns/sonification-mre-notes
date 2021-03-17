# March 17

Since yesterday did not pan out for me, I'm going to try a different approach. One of Dr. Graham's [blog posts](https://electricarchaeology.ca/2021/03/01/the-dig-we-know-where-the-bodies-are-buried/) involved the sonification of "The Sutton Hoo ship burial," by R. L. S. Bruce-Mitford. He used Sonic Pi to remix it, using this code:

```with_fx :reverb do
   in_thread do
    loop do
     notes = (ring 20,50,21,50  etc etc: these are the proportions of the different topics for the first topic)
     notes2 = (ring 6, 14, 59 etc etc)
     notes3 etc 
     notes4 etc
     use_synth :piano
     play notes, release: 0.1, amp: rand, pan: rrand(-1, 1)
     play notes2, release: 0.1, amp: rand,pan: rrand(-1, 1)
     play notes etc
     sleep 0.25
    end
   end
 end

with_fx :wobble, phase: 2 do |w|
  with_fx :echo, mix: 0.6 do
    loop do
      sample :drum_heavy_kick
      sample :bass_hit_c, rate: 0.8, amp: 0.4
      sleep 1
    end
  end
end
```

(Again, that belongs to Dr. Graham). Since yesterday was such a failure, I decided to try to copy his methods and see if I could learn what I need from that. So, I'm going to put this into Sonic Pi, and see how that goes. I'm not sure how to remix the midi file in Sonic Pi, but maybe I'll figure that out later.

Dr. Graham also answered my message re: yesterday's failures, and suggested Audacity, Garageband, and LMMS. LMMS I checked out yesterday but struggled to get SoundFonts recognized, but I'm going to try it again with this recommendation. Unfortunately I think Garageband is only for Macs, which I do not have, so Audacity it'll be! Not sure how to remix MIDI files in Audacity, since I've only ever remixed/merged mp3 files, but we'll see how it goes!

### Sonic Pi
So I just finished messing around with SonicPi, and it's great for numerical data! Lots of fun samples to add - I made a choral piece based on random numbers (because I don't have any handily-accessible data right now) using Dr. Graham's outline, and it was pretty cool. A lot of samples are very electronic though - definitely no fiddle, or any other kind of string. Lots of the sounds would be suitable for making a pseudo-sonar for 'tracking' shipwrecks along the Ottawa River though! 

So not really for remixing, but more for creating tracks based on numbers that you could then remix perhaps? Very cool, not for image sonification unless you turn the image into numbers. Which you could, but which doesn't help me with my MIDI file. Onto Audacity!

### Audacity
I've used Audacity before, 

