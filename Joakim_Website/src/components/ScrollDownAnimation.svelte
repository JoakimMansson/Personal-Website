
<span class="scroll-icon">
    <span class="scroll-icon__dot"></span>
</span>

<style>
    @keyframes scroll_2 {
  0%   { transform: translateY(0); opacity: 1; }
  25%  { opacity: 1; }
  75%  { transform: translateY(.75em); opacity: 0; }
  100% { transform: translateY(0); opacity: 0; }
}


.scroll-icon__dot {
  display: block;
  position: absolute;
  left: 50%;
  background: #fff;
  height: .5em;
  width: .5em;
  top: .6em;
  margin-left: -.25em;
  border-radius: 50%;
  transform-origin: top center;
  backface-visibility: hidden;
  animation: scroll_2 1.5s ease-out infinite;
}

.scroll-icon {
  display: block;
  position: relative;
  height: 3em;
  width: 1.5em;
  border: .25em solid #fff;
  border-radius: 1em;
}


</style>