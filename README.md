# android-docker-container

</span></code></pre></td><td class="lntd"><pre tabindex="0" class="chroma"><code class="language-bash" data-lang="bash"><span class="line"><span class="cl">sudo pacman -S docker docker-compose
</span></span><span class="line"><span class="cl">sudo systemctl <span class="nb">enable</span> --now docker
</span></span></code></pre></td></tr></tbody></button>

</span></code></pre></td><td class="lntd"><pre tabindex="0" class="chroma"><code class="language-bash" data-lang="bash"><span class="line"><span class="cl">sudo pacman -S android-tools
</span></span><span class="line"><span class="cl">sudo pacman -S scrcpy
</span></span></code></pre></td></tr></tbody><button class="copy-button" type="button" style="visibility: hidden; opacity: 0;"></table>

<code>## running redroid with custom settings (custom display for example)
docker run -itd --rm --privileged \
    --pull always \
    -v ~/data:/data \
    -p 5555:5555 \
    redroid/redroid:11.0.0-latest \
    androidboot.redroid_width=1080 \
    androidboot.redroid_height=1920 \
    androidboot.redroid_dpi=480 \
</code>

<div style="position:relative; display: flex; flex-wrap: nowrap;"> 
    <img style='position:absolute; z-index:1;' src='1.png' alt="1.png"/>
    <img style='position:absolute; z-index:1;' src='2.png' alt="2.png"/>
</div> 
