<script>
import { setTimeout } from "timers";
export default {
  name: "ReallySimpleAlert",
  props: {
    message: {
      type: String,
      default: "Hello World"
    },
    timeout: {
      type: Number,
      default: 0
    }
  },
  mounted() {
    setTimeout(() => {
      alert(this.message);
    }, this.timeout);
  }
};
</script>