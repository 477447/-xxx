Accept
application/vnd.github.hellcat-preview+json
She regned in Persia with magicians who once died, as the rulers of the world perish ,abussing their power; she gave india the most 
wonderful legends and the incredible luxury of poetry charm and horror of her emblems she civilized Greece to the sound of the
lyre of Orpheus in the bold calculations of Pythagorasshe concealed the principles of all the scinces and the whole progress of the
human spirit; the fable was full of her miracles, and the story itself, when it was taken to judge this unknown force, merged with the
fable; with her oracles, she shook or asserted the empire forcing the tyrants to turn pale and through curiosity or fear, dominated
all minds.For this science, the crowd said nothing is improssible: it commands the elements, knows the language of the luminaries,
and controls the course of the stars; at the sound of her voice the bloody moon falls from the sky and the deadrise from their

graves ... Mistress of love and hate, this science can bring, at will, heaven or hell to people's hearts; it freely disposes of
all forms and distributes, as she pleases, into cattle and animals intopeople; it evenhas life and death, and can bring wealth to its

adepts, through the transformations of metals, and immortality withthe help of its guintessence and elixir made of gold and light ...
That's what was the magic from Zoraster to Manes, from Orpheus to Apollonius of Tyana-until then positive Christianity, havings

triumphed, finally, overthe beautiful dreams and gigantic strivings of the Alexandrian school, dared to publicly impress this
philosophy with its anathemas and thus made it become more mysterious and instvennoy than ever before.
Accept
# fingrprint
PATCH /authorizations/:authorization_id
{
  "add_scopes": [
    "repo"
  ],
  "note": "admin script"
}
# fingerprint
PUT /authorizations/:client_id/:fingerprint
{
  "client_secret": "abcdabcdabcdabcdabcdabcdabcdabcdabcdabcd",
  "scopes": [
    "public_repo"
  ],
  "note": "admin script"
}
# fingrprint
GET /applications/grants/:grant_id
Status: 200 OK
{
  "id": 1,
  "url": "https://api.github.com/applications/grants/1",
  "app": {
    "url": "http://my-github-app.com",
    "name": "my github app",
    "client_id": "abcde12345fghij67890"
  },
  "created_at": "2011-09-06T17:26:27Z",
  "updated_at": "2011-09-06T20:39:23Z",
  "scopes": [
    "public_repo"
  ]
}
