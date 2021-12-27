
<script>
import "./tree.css";
export default {
  data() {
    return {};
  },
  render() {
    const len = [new Array(3), new Array(4)];
    let item = len.map((i) => {
      let line = i.map(() => {
        return (
          <p
            style={
              "width:32px;height: 32px;background: green;display:inline-block;margin-right:2px"
            }
            className={"leaf"}
          ></p>
        );
      });
      return line;
    });
    return <div className={"tree"}>{item}</div>;
  },
};
</script>
<style lang="css">
.leaf {
  width: 20px;
  height: 20px;
  background: green;
}
</style>
