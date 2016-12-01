# python00
python study , examples, test

## Two ++
Two Content

  Two Space Before
Two Space Content 

    Four Space Before
Four Space Content 

- List1
- List2
- List3

### Three ###
Three content

Use the **`print()`** function.

Code here use 4 spaces

    def testCodeBlock():
        print( "run code" )
    #_ def testCodeBlock

Code here use tag pre
<pre class="prettyprint linenums">
def testCodeBlock():
     print( "run code" )
#_ def testCodeBlock
</pre>

Code here use tag code
<code>
def spCmd( cmd_in=None ):
	print( "--- spCmd start ---" )
	if( cmd_in is None or len(cmd_in) <= 0 ):
		print( "spCmd: command is empty" )
		out.flush()
		return 0
	#_ if
	try:
		#out_bytes = subprocess.check_output( cmd_in )
		#out_bytes = subprocess.check_output( cmd_in, shell=True, stderr=subprocess.STDOUT )
		out_bytes = subprocess.check_output( cmd_in, stderr=subprocess.STDOUT )
		##print("[",out_bytes.decode("mbcs" ), "]" )
		print( "[", out_bytes.decode("utf_8"), "]" )
	except subprocess.CalledProcessError as e:
		out_bytes = e.output  # Output generated before error
		code = e.returncode  # Return code
		print( "code=", code, "[", out_bytes, "]" )
		out.flush()
		return 0
	except:
		print( "Unexpected error:", sys.exc_info()[0] )
		out.flush()
		return 0
	#_ try
	return 1
#_ def spCmd
</code>

+ item 1
+ item 2
+ item 3

#### Link to self [python00][]

## Show Code
<script src="https://gist.github.com/arioso27/c5d9879c3b91e1366b7d36c859f1a0af.js"></script>


[python00]: https://github.com/arioso27/python00 "python00 URL"

<script src="https://cdn.rawgit.com/google/code-prettify/master/loader/run_prettify.js"></script>
