<script lang="ts">
    import { TableOfContents, tocCrawler } from "@skeletonlabs/skeleton";
</script>

<div>
    <div>
        <TableOfContents class="sticky top-10"/>
    </div>
    <div use:tocCrawler={{ mode: 'generate' }} class="p-4 space-y-4">
        <h1 class="h1">About</h1>
        <div>
            <h2 class="h2">Introduction</h2>
            <h3 class="h3">What is a GGG?</h3>
            <p>Green Gas Giants (GGGs) are a rare gas giant subtype in Elite: Dangerous. These planets differ from the standard gas giants as they show unique colors in their
                upper atmospheres, most notably bright neon green, for which they are named. Universal Cartographics attributes these vibrant colors to exotic bioluminescent
                radioplankton that absorb energy from the gas giant's intese radiation flux. Their colors and cloud patterns vary wildly between classes, as well as within a 
                given class.
                <br /><br />
                In reality however, these green planets were not originally meant to be in the game, and are likely the result of an oversight in the color generation of the 
                planet. There are theories about how some gas giants turn green, but overall there is currently no consistent method of predicting if a gas giant will be green or not.
            </p>
            <h3 class="h3">History</h3>
            <p>The first Green Gas Giant was discovered in 3301 by CMDR Kelly Eldridge. Its location was originally lost for 7 years, eventually being rediscovered by the <em>At The Eldritch Gate</em> expedition 
             in the Shaulai DL-P d5-274 system. The next four Green Gas Giants discovered were all gas giants that bore either water-based for ammonia-based airborne life within their atmospheres, so it was
             originally believed that only those gas giants were able to turn green. That was the case until late 3303 when a Class III Green Gas Giant was discovered in the Floasly TE-X d2-25 system.
             <br /><br />
             From then on, the discovered GGG count steadily rose through the years, and almost all gas giant classes have at least one confirmed green variant. CMDRs have been speculating
             on the cause of this strange flourescent coloration, taking into account parent star types or atmospheric composition, but no definite pattern could be detected between them. That was 
             until 3309 when CMDR Arcanic discovered a relationship between certain gas giant classes and certain surface temperatures. His theory was that both Water-Based Life and Class III gas giants turn green when their
            surface temperatures match specific numbers, down to six significant figures. A short while later, two Water-Based Life Green Gas Giants were rediscovered using this method. However, this theory 
            was not consistent for other classes; Multiple gas giants were found that shared a specific surface temperature with a Green Gas Giant that turned out not to be green. Alas, the mystery of GGG
            generation continues to allude us. 
            </p>
            <h3 class="h3">GGG Classes</h3>
            <p>
                Almost all gas giant classes in the game have a known GGG variant, and they are the following:
            </p>
                <ul class="list-disc pl-5">
                    <li><a href='/'>Class I</a></li>
                    <li><a href='/'>Class II</a></li>
                    <li><a href='/'>Class III</a></li>
                    <li><a href='/'>Class IV</a></li>
                    <li><a href='/'>Gas Giant with Water-Based Life</a></li>
                    <li><a href='/'>Gas Giant with Ammonia-Based Life</a></li>
                    <li><a href='/'>Water Giant</a></li>
                </ul>
                <br />
            <p>The following gas giant classes do <strong>not</strong> currently have a known GGG variant:</p>
                <ul class="list-disc pl-5">
                    <li>Class V</li>
                    <li>Helium-Rich Gas Giant</li>
                    <li>Helium Gas Giant</li>
                </ul>
            <h2 class="h2">Identifying a GGG</h2>
            <p>When out exploring in the black, there are multiple ways to confirm whether you have come across a Green Gas Giant or not. Below are all the methods you
                can use to determine if you have done so.
            </p>
        </div>
        <div class="card p-4 flex">
            <div>
            <h3 class="h3">FSS</h3>
            <p>GGGs do not have a special area on the FSS spectrum; A Class I GGG will be located where normal Class Is usually show up. Viewing a Green Gas Giant on the FSS easily resolves the bright cloud colors in its upper atmosphere. Keep in mind that some planets have more discolored regions than
                others. It might not be immediately obvious where on the planet the green colors are at. Some do not have any noticeable green <em>at all</em>
            </p>
            </div>
            <img src="" alt="A Green Gas Giant in the FSS Scanner" />
        </div>
        <div class="card p-4 flex">
            <div>
            <h3 class="h3">Codex Alerts</h3>
            <p>The first time you come across a GGG of a certain class in a region, you will be notified of your discovery via a codex notification. This is the quickest way to confirm if a 
                gas giant is green or not. However, this only works once each class. If you visit another Green Gas Giant of the same type in the same region, you will <strong>NOT</strong> be notified, which might make you potentially miss a new GGG if it isn't immediately viusally apparent.
                <strong>NOTE:</strong> For whatever reason, Green Gas Giants with Water-based Life do NOT have a codex entry, it is instead taken by Ammonia-Based Life GGGs.
            </p>
            </div>
            <img src="" alt="A Green Gas Giant codex notification" />
        </div>
        <div class="card p-4 flex">
            <div>
            <h3 class="h3">Planet Description</h3>
            <p>
                Each GGG's planetary description in the system map has been modified to reference its green appearance. The extra text appended to the normal description usually starts
                with "This particular gas giant exhibits vivid coloration..." or "Luminous vapour can be detected in the planet's upper atmosphere..."
            </p>
            </div>
            <img src="" alt="Planet description of a GGG" />
        </div>
        <div class="card p-4 flex">
            <div>
            <h3 class="h3">"Green Light"</h3>
            <p>Some GGGs display a bright green "pinprick" of light when far away. It is unknown why only some planets do this and some do not.</p>
            </div>
            <img src="" alt="A green light cast from a GGG in-system" />
        </div>
        <div class="card p-4 flex"> TODO: Fix the flex display on this card thx
            <div>
                <div>
                <h3 class="h3">Surface Temperature</h3>
                 <p>Water-Based Life GGGs and Class III GGGs have certain temperatures that are confirmed to always make a gas giant green. Using third-party tools such as <em>Elite: Dangerous Observatory</em>,
                custom criteria can be written to scan the game journal files and can notify you if a gas giant matches a matching temperature. 
                </p>
                <br />
                <!-- <div class="flex">
                    <div>
                        <span>GGGWBL Temps:</span>
                        <ul class="list-disc pl-5">
                        <li>158.000000K</li>
                        <li>176.666641K</li>
                         <li>176.666656K</li>
                         <li>176.666672K</li>
                        <li>176.666687K</li>
                        <li>217.499985K</li>
                        </ul>
                    </div>
                    <div>
                        <span>Class III Temps:</span>
                        <ul class="list-disc pl-5">
                        <li>370.000000K</li>
                        <li>550.000000K</li>
                         <li>580.000000K</li>
                        <li>610.000000K</li>
                        <li>640.000000K</li>
                        <li>700.000000K</li>
                        </ul>
                    </div>
                    </div> -->
                    <img src="" alt="Confirmed GGG Temperature Notification in ED:O" />
                </div>
            </div>
        </div>
        <div class="card p-4 flex">
            <div>
            <h3 class="h3">K-10 Type Anomalies</h3>
            <p>If you are travelling within either the Galactic Centre or Ryker's Hope galactic regions, you have the chance to encounter K-10 Type anomalies. These anomalies
                only spawn when Green Gas Giants are present within a system. These will show up as Notable Stellar Phenomena, which are immediately displayed in your Nav Panel
                upon system arrival from hyperspace. This can make searching for GGGs in this region super efficient, as if there are no NSPs present in your Nav Panel, there is no GGG in the current system.
            </p>
            </div>
            <img src="" alt="K-10 Type Anomalies" />
        </div>
    </div>
</div>
