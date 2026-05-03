# snow.css1
body::before {
  content: "";
  position: fixed;
  top: -100%;
  left: 0;
  width: 100%;
  height: 200%;

  background-image:
    radial-gradient(#aaa 1px, transparent 1px),
    radial-gradient(#bbb 1px, transparent 1px),
    radial-gradient(#999 2px, transparent 2px);

  background-size: 80px 80px, 120px 120px, 160px 160px;
  opacity: 0.3;

  animation: snow 12s linear infinite;
}

@keyframes snow {
  0% { transform: translateY(-50%); }
  100% { transform: translateY(0%); }
}