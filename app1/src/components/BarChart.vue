<script>
import { Bar } from "vue-chartjs";

export default {
  extends: Bar,
  mounted() {
    this.renderChart(
      {
        labels: [
          "January",
          "February",
          "March",
          "April",
          "May",
          "June",
          "July",
          "August",
          "September",
          "October",
          "November",
          "December"
        ],
        datasets: [
          {
            label: "Data Sync",
            backgroundColor: "#DC143C",
            data: [40, -20, 12, 39, -10, 40, 39, 80, -40, 20, 12, 11]
          }
        ]
      },
      { responsive: true, maintainAspectRatio: false }
    );
  }
};
</script>

