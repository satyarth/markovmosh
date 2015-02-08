# Markov Chain Based Text Generator

This allows you to create a redis-backed markov chain class for use in, well, anything. Personally, I'm using it to generate hilarious mashups of bash scripting guides and Wu-Tang Clan lyrics, but you can do what you want with it.

## Dependencies

* python2-redis
* redis server running on localhost

## Usage

Generate a random message from your corpus

```
$ ./markovmosh.py
```

Give it a seed of chain-length (hardcoded in the file, change if you want)

```
$ ./markovmosh.py -s 'wu-tang clan'
```

Train your bot (add text files to its chain database). This command supports shell globbing and multiple arguments.

```
$ ./markovmosh.py -t /path/to/my/text/file/dir/*
```

Search for a key in the bot's memory

```
$ ./markovmosh.py -k 'killa bees'
```

Wipe your bot's memory

```
$ ./markovmosh.py -f
```

Get advanced help

```
$ ./markovmosh.py -h
```

## Examples

##### "Pride & Prejudice" + "36 Chambers" + "Straight Outta Compton"

"Sophisticated motherfuckers hear what has happened this morning? Mr. Collins by Janes letter last wednesday that her cousins manners were very unfit to have his errors made public might ruin him in company four times. This is quite shocking!"

"So fuck the police, always got somethin stupid to say or sense of obligation for the long-expected ball at Netherfield."
