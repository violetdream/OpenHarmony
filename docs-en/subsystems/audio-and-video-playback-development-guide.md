# Audio and Video Playback Development Guide<a name="EN-US_TOPIC_0000001051930589"></a>

## When to Use<a name="section186634310418"></a>

Audio and video playback is a process in which audio and video files or audio and video stream data is decoded and played by using an output device, and a playback task is managed.

## Available APIs<a name="section125479541744"></a>

The audio and video playback APIs are described as follows. For details about the APIs, see the API reference document.

**Table  1**  Audio and Video Playback APIs

<a name="table1139164071320"></a>
<table><thead align="left"><tr id="row85501040111310"><th class="cellrowborder" valign="top" width="15.959999999999999%" id="mcps1.2.4.1.1"><p id="p755044051316"><a name="p755044051316"></a><a name="p755044051316"></a>API</p>
</th>
<th class="cellrowborder" valign="top" width="47.77%" id="mcps1.2.4.1.2"><p id="p1755024018131"><a name="p1755024018131"></a><a name="p1755024018131"></a>Function</p>
</th>
<th class="cellrowborder" valign="top" width="36.27%" id="mcps1.2.4.1.3"><p id="p8550134015131"><a name="p8550134015131"></a><a name="p8550134015131"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row17550440151310"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p6550440111312"><a name="p6550440111312"></a><a name="p6550440111312"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p65504403132"><a name="p65504403132"></a><a name="p65504403132"></a>static Player *CreatePlayer();</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p115501540191319"><a name="p115501540191319"></a><a name="p115501540191319"></a>Creates a <strong id="b438710876105433"><a name="b438710876105433"></a><a name="b438710876105433"></a>Player</strong> instance.</p>
</td>
</tr>
<tr id="row14550164011132"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p55505406135"><a name="p55505406135"></a><a name="p55505406135"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p15550240191312"><a name="p15550240191312"></a><a name="p15550240191312"></a>int32_t SetSource(const Source &amp;source);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p125502402132"><a name="p125502402132"></a><a name="p125502402132"></a>Set playback source</p>
</td>
</tr>
<tr id="row155044001318"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p255064021310"><a name="p255064021310"></a><a name="p255064021310"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p10550104014132"><a name="p10550104014132"></a><a name="p10550104014132"></a>int32_t Prepare();</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p155503406138"><a name="p155503406138"></a><a name="p155503406138"></a>Prepares the playback environment and buffers media data.</p>
</td>
</tr>
<tr id="row165502040141313"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p3550174081313"><a name="p3550174081313"></a><a name="p3550174081313"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p9550144011310"><a name="p9550144011310"></a><a name="p9550144011310"></a>int32_t Play();</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p255094041314"><a name="p255094041314"></a><a name="p255094041314"></a>Starts playback.</p>
</td>
</tr>
<tr id="row855064010130"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p3550840151318"><a name="p3550840151318"></a><a name="p3550840151318"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p195501409137"><a name="p195501409137"></a><a name="p195501409137"></a>bool IsPlaying()</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p255114020137"><a name="p255114020137"></a><a name="p255114020137"></a>Determines whether the playback is in progress.</p>
</td>
</tr>
<tr id="row1555111402135"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p05511840151313"><a name="p05511840151313"></a><a name="p05511840151313"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p16551340151314"><a name="p16551340151314"></a><a name="p16551340151314"></a>int32_t Pause();</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p14551164021311"><a name="p14551164021311"></a><a name="p14551164021311"></a>Pauses playback.</p>
</td>
</tr>
<tr id="row155511740111315"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p185515403139"><a name="p185515403139"></a><a name="p185515403139"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p19551184031318"><a name="p19551184031318"></a><a name="p19551184031318"></a>int32_t Stop();</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p555154041312"><a name="p555154041312"></a><a name="p555154041312"></a>Stops playback.</p>
</td>
</tr>
<tr id="row1255118400138"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p6551114081317"><a name="p6551114081317"></a><a name="p6551114081317"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p8551154015135"><a name="p8551154015135"></a><a name="p8551154015135"></a>int32_t Rewind(int_64 mSeconds, int32_t mode);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p1255184019138"><a name="p1255184019138"></a><a name="p1255184019138"></a>Change the playback position.</p>
</td>
</tr>
<tr id="row195511640141312"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1455164061314"><a name="p1455164061314"></a><a name="p1455164061314"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p5551340151313"><a name="p5551340151313"></a><a name="p5551340151313"></a>int32_t SetVolume(float leftVolume, float rightVolume);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p19551940181320"><a name="p19551940181320"></a><a name="p19551940181320"></a>Sets the volume of the audio-left and audio-right channels.</p>
</td>
</tr>
<tr id="row19551144015130"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p2055113408131"><a name="p2055113408131"></a><a name="p2055113408131"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p1055124011314"><a name="p1055124011314"></a><a name="p1055124011314"></a>int32_t SetVideoSurface(Surface *surface)</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p1355104041311"><a name="p1355104041311"></a><a name="p1355104041311"></a>Setting the Playback Window</p>
</td>
</tr>
<tr id="row1355174010135"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p85511140161313"><a name="p85511140161313"></a><a name="p85511140161313"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p155114401137"><a name="p155114401137"></a><a name="p155114401137"></a>int32_t EnableSingleLooping(bool loop)</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p05513403130"><a name="p05513403130"></a><a name="p05513403130"></a>Single-song repeat</p>
</td>
</tr>
<tr id="row185511040151319"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p3552124010139"><a name="p3552124010139"></a><a name="p3552124010139"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p6552144021318"><a name="p6552144021318"></a><a name="p6552144021318"></a>bool IsSingleLooping();</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p555220403134"><a name="p555220403134"></a><a name="p555220403134"></a>Determines whether to play the video cyclically.</p>
</td>
</tr>
<tr id="row24941622111618"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1555214041314"><a name="p1555214041314"></a><a name="p1555214041314"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p1655294011317"><a name="p1655294011317"></a><a name="p1655294011317"></a>int32_t GetCurrentTime(int64_t &amp;time) const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p255234031315"><a name="p255234031315"></a><a name="p255234031315"></a>Obtains the current playback duration.</p>
</td>
</tr>
<tr id="row655224015139"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p165520406137"><a name="p165520406137"></a><a name="p165520406137"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p7552164071320"><a name="p7552164071320"></a><a name="p7552164071320"></a>int32_t GetDuration(int64_t &amp;duration) const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p17552640141312"><a name="p17552640141312"></a><a name="p17552640141312"></a>Obtains the total playback duration.</p>
</td>
</tr>
<tr id="row11552194019131"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p955214013132"><a name="p955214013132"></a><a name="p955214013132"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p655234018131"><a name="p655234018131"></a><a name="p655234018131"></a>int32_t GetVideoWidth(int32_t &amp;videoWidth);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p12552174081314"><a name="p12552174081314"></a><a name="p12552174081314"></a>Obtains the width of a video source.</p>
</td>
</tr>
<tr id="row8552164013134"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p125525404136"><a name="p125525404136"></a><a name="p125525404136"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p13552114011316"><a name="p13552114011316"></a><a name="p13552114011316"></a>int32_t GetVideoHeight(int32_t &amp;videoHeight);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p14552134011138"><a name="p14552134011138"></a><a name="p14552134011138"></a>Obtains the height of a video source.</p>
</td>
</tr>
<tr id="row6552340181312"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1155244017138"><a name="p1155244017138"></a><a name="p1155244017138"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p1955374031313"><a name="p1955374031313"></a><a name="p1955374031313"></a>int32_t Reset();</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p1553124061317"><a name="p1553124061317"></a><a name="p1553124061317"></a>Restores the player to the initial state.</p>
</td>
</tr>
<tr id="row6553134021311"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1655314021316"><a name="p1655314021316"></a><a name="p1655314021316"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p13553194018132"><a name="p13553194018132"></a><a name="p13553194018132"></a>int32_t Release();</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p455354018139"><a name="p455354018139"></a><a name="p455354018139"></a>Releasing Player Resources</p>
</td>
</tr>
<tr id="row25531940151318"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p95531440191318"><a name="p95531440191318"></a><a name="p95531440191318"></a>Player</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p1955317400131"><a name="p1955317400131"></a><a name="p1955317400131"></a>void SetPlayerCallback(const std::shared_ptr&lt;PlayerCallback&gt; &amp;cb);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p135530402139"><a name="p135530402139"></a><a name="p135530402139"></a>Sets the playback callback function.</p>
</td>
</tr>
<tr id="row26841936205916"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p155531940171317"><a name="p155531940171317"></a><a name="p155531940171317"></a>Source</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p1955314012137"><a name="p1955314012137"></a><a name="p1955314012137"></a>Source(const std::string&amp; uri);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p755314031315"><a name="p755314031315"></a><a name="p755314031315"></a>Creating a Source Instance Based on the URI</p>
</td>
</tr>
<tr id="row1839749195917"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p13553040181316"><a name="p13553040181316"></a><a name="p13553040181316"></a>Source</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p125538401138"><a name="p125538401138"></a><a name="p125538401138"></a>Source(const std::string &amp;uri, const std::map&lt;std::string, std::string&gt; &amp;header);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p35533406130"><a name="p35533406130"></a><a name="p35533406130"></a>Creating a Source Instance Based on the URI and URI Header</p>
</td>
</tr>
<tr id="row16713165319598"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p195531740141316"><a name="p195531740141316"></a><a name="p195531740141316"></a>Source</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p655310403132"><a name="p655310403132"></a><a name="p655310403132"></a>Source(const std::shared_ptr&lt;StreamSource&gt; &amp;stream, const Format &amp;formats);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p05536401138"><a name="p05536401138"></a><a name="p05536401138"></a>Creating a Source Instance Based on Flows</p>
</td>
</tr>
<tr id="row39004563590"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p15531340191312"><a name="p15531340191312"></a><a name="p15531340191312"></a>Source</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p13553174091318"><a name="p13553174091318"></a><a name="p13553174091318"></a>SourceType GetSourceType() const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p1455354016136"><a name="p1455354016136"></a><a name="p1455354016136"></a>Obtains the source type.</p>
</td>
</tr>
<tr id="row15429101008"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1655434018139"><a name="p1655434018139"></a><a name="p1655434018139"></a>Source</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p7554154013137"><a name="p7554154013137"></a><a name="p7554154013137"></a>const std::string &amp;GetSourceUri() const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p1855414071310"><a name="p1855414071310"></a><a name="p1855414071310"></a>Obtains the audio and video URIs.</p>
</td>
</tr>
<tr id="row12357142103"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1554124015132"><a name="p1554124015132"></a><a name="p1554124015132"></a>Source</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p12554134016134"><a name="p12554134016134"></a><a name="p12554134016134"></a>const std::map&lt;std::string, std::string&gt; &amp;GetSourceHeader() const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p3554124091318"><a name="p3554124091318"></a><a name="p3554124091318"></a>Obtains the audio and video URI headers.</p>
</td>
</tr>
<tr id="row17477411011"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p105540409134"><a name="p105540409134"></a><a name="p105540409134"></a>Source</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p1355434014138"><a name="p1355434014138"></a><a name="p1355434014138"></a>const std::shared_ptr&lt;StreamSource&gt; &amp;GetSourceStream() const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p455415408132"><a name="p455415408132"></a><a name="p455415408132"></a>Obtaining Audio and Video Streams</p>
</td>
</tr>
<tr id="row19135971706"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p257064871110"><a name="p257064871110"></a><a name="p257064871110"></a>Source</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p151191016151214"><a name="p151191016151214"></a><a name="p151191016151214"></a>const Format &amp;GetSourceStreamFormat() const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p14257126131210"><a name="p14257126131210"></a><a name="p14257126131210"></a>Obtains the audio and video stream formats.</p>
</td>
</tr>
<tr id="row1543179104"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p255412409135"><a name="p255412409135"></a><a name="p255412409135"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p655454001314"><a name="p655454001314"></a><a name="p655454001314"></a>bool PutIntValue(const std::string &amp;key, int32_t value);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p205661711619"><a name="p205661711619"></a><a name="p205661711619"></a>Sets the metadata of the integer type.</p>
</td>
</tr>
<tr id="row695314111204"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p655454019138"><a name="p655454019138"></a><a name="p655454019138"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p1554840111319"><a name="p1554840111319"></a><a name="p1554840111319"></a>bool PutLongValue(const std::string &amp;key, int64_t value);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p230317337163"><a name="p230317337163"></a><a name="p230317337163"></a>Sets the metadata of the long integer type.</p>
</td>
</tr>
<tr id="row3518133213019"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1855434031312"><a name="p1855434031312"></a><a name="p1855434031312"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p1555484014139"><a name="p1555484014139"></a><a name="p1555484014139"></a>bool PutFloatValue(const std::string &amp;key, float value);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p12391147111614"><a name="p12391147111614"></a><a name="p12391147111614"></a>Sets the metadata of the single-precision floating-point type.</p>
</td>
</tr>
<tr id="row176434351308"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p655534031317"><a name="p655534031317"></a><a name="p655534031317"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p5555640111320"><a name="p5555640111320"></a><a name="p5555640111320"></a>bool PutDoubleValue(const std::string &amp;key, double value);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p185881525191711"><a name="p185881525191711"></a><a name="p185881525191711"></a>Sets the metadata of the double-precision floating-point type.</p>
</td>
</tr>
<tr id="row9476163810013"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p3555154017133"><a name="p3555154017133"></a><a name="p3555154017133"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p3555124015133"><a name="p3555124015133"></a><a name="p3555124015133"></a>bool PutStringValue(const std::string &amp;key, const std::string &amp;value);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p16021743131719"><a name="p16021743131719"></a><a name="p16021743131719"></a>Sets the metadata of the character string type.</p>
</td>
</tr>
<tr id="row879515406015"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p15551540181313"><a name="p15551540181313"></a><a name="p15551540181313"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p19555164041313"><a name="p19555164041313"></a><a name="p19555164041313"></a>bool GetIntValue(const std::string &amp;key, int32_t &amp;value) const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p435725714171"><a name="p435725714171"></a><a name="p435725714171"></a>Obtains the metadata value of the integer type.</p>
</td>
</tr>
<tr id="row462919431104"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1655544021318"><a name="p1655544021318"></a><a name="p1655544021318"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p0555194031314"><a name="p0555194031314"></a><a name="p0555194031314"></a>bool GetLongValue(const std::string &amp;key, int64_t &amp;value) const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p7330132141811"><a name="p7330132141811"></a><a name="p7330132141811"></a>Obtains the metadata value of the long integer type.</p>
</td>
</tr>
<tr id="row1797513451904"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1655624011319"><a name="p1655624011319"></a><a name="p1655624011319"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p155567401134"><a name="p155567401134"></a><a name="p155567401134"></a>bool GetFloatValue(const std::string &amp;key, float &amp;value) const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p080203817189"><a name="p080203817189"></a><a name="p080203817189"></a>Obtains the metadata value of the single-precision floating-point type.</p>
</td>
</tr>
<tr id="row012319491603"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p855694013132"><a name="p855694013132"></a><a name="p855694013132"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p10556124015132"><a name="p10556124015132"></a><a name="p10556124015132"></a>bool GetDoubleValue(const std::string &amp;key, double &amp;value) const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p116117558189"><a name="p116117558189"></a><a name="p116117558189"></a>Obtains the metadata value of the double-precision floating-point type.</p>
</td>
</tr>
<tr id="row22531651901"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p1855604081314"><a name="p1855604081314"></a><a name="p1855604081314"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p9556840171310"><a name="p9556840171310"></a><a name="p9556840171310"></a>bool GetStringValue(const std::string &amp;key, std::string &amp;value) const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p6495161451914"><a name="p6495161451914"></a><a name="p6495161451914"></a>Obtains the metadata value of the character string type.</p>
</td>
</tr>
<tr id="row552743019"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p165563405133"><a name="p165563405133"></a><a name="p165563405133"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p4556134061315"><a name="p4556134061315"></a><a name="p4556134061315"></a>const std::map&lt;std::string, FormatData *&gt; &amp;GetFormatMap() const;</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p3379195115711"><a name="p3379195115711"></a><a name="p3379195115711"></a>Obtain the Map table of the format.</p>
</td>
</tr>
<tr id="row127651251115"><td class="cellrowborder" valign="top" width="15.959999999999999%" headers="mcps1.2.4.1.1 "><p id="p16556240111315"><a name="p16556240111315"></a><a name="p16556240111315"></a>Format</p>
</td>
<td class="cellrowborder" valign="top" width="47.77%" headers="mcps1.2.4.1.2 "><p id="p195561240111317"><a name="p195561240111317"></a><a name="p195561240111317"></a>bool CopyFrom(const Format &amp;format);</p>
</td>
<td class="cellrowborder" valign="top" width="36.27%" headers="mcps1.2.4.1.3 "><p id="p185953195717"><a name="p185953195717"></a><a name="p185953195717"></a>Copies all content from a format instance.</p>
</td>
</tr>
</tbody>
</table>

## Limitations and Constraints<a name="section1165911177314"></a>

When the input source is an audio or video stream, the playback progress cannot be controlled and the file duration cannot be obtained.

## How to Develop<a name="section34171333656"></a>

1.  Implement the PlayerCallback callback function for event processing.

    ```
    class TestPlayerCallback : public PlayerCallback{ 
        void OnPlayBackComplete() override 
        { 
    // The implementation code is used to process the event that the file playback is complete.
        } 
        void OnError(int32_t errorType, int32_t errorCode) override 
        { 
    // Implement the code processing error event.
        } 
        void OnInfo(int type, int extra) override 
        { 
    //Implement the code to process common events.
        } 
        void OnRewindToComplete() override 
        { 
    //Implement the event that the code processing progress control is complete.
        } 
    };
    
    ```

2.  Create a player instance, set the playback source, and start playback.

    ```
    Player *player = Player::CreatePlayer(); 
    std::shared_ptr<PlayerCallback> callback = std::make_shared<TestPlayerCallback>(); 
    player->SetPlayerCallback(callback);// Set player callback.
    std::string uri(filePath);// filePath is the local file path.
    Source source(uri);//Save the URI to the source instance.
    player->SetSource(source);//Set the source to the player.
    player->SetVideoSurface(surface);//Set the playback window.
    player->Prepare(); // Prepare for the playback.
    player->Play(); //Starts playback.
    ```

3.  Perform playback control based on the scenario.

    ```
    player->SetVolume(lvolume, rvolume);//Set the left and right sound channels.
    player->EnableSingleLooping(true);// Set cyclic playback.
    player->Pause(); //Pause.
    player->Play(); //Continue the playback.
    ```

4.  Release resources after the playback task is complete.

    ```
    player->Stop(); //Stop the playback.
    player->Release(); // Release resources.
    ```


