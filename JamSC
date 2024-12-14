(
p = ProxySpace(
	server: s.boot,
	clock: t = TempoClock(90/60).permanent_(true),
).push;
p.fadeTime_(4);
p.quant_(4);
)

a = ();
a.fl0 = Buffer.read(s, "/Users/christiandavid/Documents/sc/arpegio.wav");
~l.fadeTime_(4).play;
~l = {PlayBuf.ar(2, a.fl0, LFNoise1.kr(4).range(0.5, 1.5), Impulse.kr(0.25)) * 0.5}
~l.release;

~z.play(fadeTime: 4);
~z.stop(4);
(~z = {SinOsc.ar([Rand(222, 333), Rand(444, 555), Rand(666, 777)], mul: SinOsc.kr(Rand(6, 32), 0, 0.1)) * LFPulse.kr([Rand(1, 12),Rand(1, 12),Rand(1, 12)])
};)

~b.play(fadeTime: 4);
~b.stop(4);
(~b = {PinkNoise.ar(0.06 ! 2) * LFSaw.kr(300)};)

~c.play(fadeTime: 4);
~c.stop(4);
(~c = {LPF.ar(Saw.ar([60, 61] * Rand(-2, 5).midiratio, mul: 0.1), 750)};)

~d.play(fadeTime: 4);
~d.stop(4);
(~d = {Dust.ar(128!2, mul: 0.04)};)

~e.play(fadeTime: 4);
~e.stop(4);
(~e = {Impulse.ar([10, 10.1], mul: 0.5) * SinOsc.kr(0.2, 3pi/2).exprange(0.1, 1)};)

~f.play(fadeTime: 4);
~f.stop(4);
(~f = {
	var sig, mod;
	mod = SinOsc.ar(MouseX.kr(300, 500, 100), mul: MouseY.kr(1, 10000, 1));
	sig = SinOsc.ar(Rand(300, 500) + mod, mul: 0.2 ! 2);
	sig = sig * LFNoise1.kr(8!2).exprange(0.2, 0.8);
};)

~g.play(fadeTime: 4);
~g.stop(4);
(~g = {LFTri.ar([Rand(250, 300), Rand(300, 350)] + SinOsc.ar(Rand(6, 12)).bipolar(Rand(8, 16)), mul: 0.05!2)};)
