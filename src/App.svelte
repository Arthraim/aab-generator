<script>
  var a = "香";
  var b = "鸡";
</script>

<main>
  <p>
    输入一个<input type='text' on:change="{v => {a = v.target.value}}" placeholder="词" value={a} />，
    再输入一个<input type='text' width=1 on:change="{v => {b = v.target.value}}" placeholder="物" value={b} />
    <br>
    得到一个<span class="result">{a||"哎"}{a||"哎"}{b||"哔"}</span>
  </p>
</main>

<style>
  p {
    font-size: 26px;
  }
  input {
    border: none;
    border-bottom: 1px solid black;
    width: 30px;
    font-size: 26px;
    font-weight: 500;
    text-align: center;
  }
  .result {
    font-weight: 500;
  }
</style>