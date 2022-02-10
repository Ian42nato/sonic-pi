# sonic-pi
2.times do
  sample :drum_snare_soft
  sleep 2
end
sleep 0.5
4.times do
  sample :drum_heavy_kick, amp: 2
  sleep 1
end
live_loop :one do
  sample :drum_snare_soft
  sleep 1
end
live_loop :two do
  sample :drum_heavy_kick, amp: 2
  sleep 1
end
live_loop :three do
  sample :drum_cymbal_closed
  sleep 0.5
end
sleep 4
sample :drum_splash_hard, sustain: 3
sample :drum_cymbal_hard
sample :drum_cowb
sleep 5
sample :drum_roll
sleep 1
sample :drum_heavy_kick
