###For this run, encouraged by small successes, I expanded the training data to a period far outside the Tang, incorporating classical Chinese poetry translations from several sources.

This largely worked, with some caveats. Some poems came with lengthy footnotes or preludes describing the context in which the poet worked. Various sources had different ways of annotating formats, splitting titles, and even the length of the poem: some were five-six times larger than the the average poem from the first Tang set. 

Good samples: 

'ON A MOONLIGHT NIGHT

Far off in Fuzhou she is watching the moonlight,
Watching it alone from the window of her chamber-
For our boy and girl, poor little babes,
Are too young to know where the Capital is.
Her cloudy hair is sweet with mist,
Her jade-white shoulder is cold in the moon.
...When shall we lie again, with no more tears,
Watching this bright light on our screen?'

'AT PARTING

'I dismount from my horse and I offer you a cup of wine
And I ask you where you are going and why.
And you answer: "I am discontent
And would rest at the foot of the southern mountain.
So give me leave and ask me no questions.
White clouds pass there without end."'

'TO QIWU QIAN BOUND HOME
AFTER FAILING IN AN EXAMINATION

In a happy reign there should be no hermits;
The wise and able should consult together....
So you, a man of the eastern mountains,
Gave up your life of picking herbs
And came all the way to the Gate of Gold --
But you found your devotion unavailing.
...To spend the Day of No Fire on one of the southern rivers,
You have mended your spring clothes here in these northern cities.
I pour you the farewell wine as you set out from the capital --
Soon I shall be left behind here by my bosomfriend.
In your sail-boat of sweet cinnamon-wood
You will float again toward your own thatch door,
Led along by distant trees
To a sunset shining on a far-away town.
...What though your purpose happened to fail,
Doubt not that some of us can hear high music.'

At samples = 600 the model is clearly overfitting. For exammple:

'TAKING LEAVE OF FRIENDS ON MY WAY TO HUAZHOU

In the second year of Zhide, I escaped from the capital through the Gate of Golden Light and went to Fengxiang. In the first year of Qianyuan, I was appointed as official to Huazhou from my former post of Censor. Friends and relatives gathered and saw me leave by the same gate. And I wrote this poem.

This is the road by which I fled,
When the rebels had reached the west end of the city;
And terror, ever since, has clutched at my vitals
Lest some of my soul should never return.
...The court has come back now, filling the capital;
But the Emperor sends me away again.
Useless and old, I rein in my horse
For one morning and the ending of an adventure.'

This sample above is virtually identical to the original, which is prefaced by:

'In the second year of Zhide, I escaped from the capital through the Gate of Golden Light and went to Fengxiang. In the first year of Qianyuan, I was appointed as official to Huazhou from my former post of Censor. Friends and relatives gathered and saw me leave by the same gate. And I wrote this poem.

This is the road by which I fled, 
When the rebels had reached the west end of the city; 
And terror, ever since, has clutched at my vitals 
Lest some of my soul should never return. 
...The court has come back now, filling the capital; 
But the Emperor sends me away again. 
Useless and old, I rein in my horse 
For one last look at the thousand gates.'

Likewise: 

'Flowers are shadowed, the palace darkens, 
Birds twitter by for a place to perch; 
Heaven's ten thousand windows are twinkling, 
And nine cloud-terraces are gleaming in the moonlight. 
...While I wait for the golden lock to turn, 
I hear jade pendants tinkling in the wind.... 
I have a petition to present in the morning, 
All night I ask what time it is. '

So this is useful at figuring out how much training is too much.
