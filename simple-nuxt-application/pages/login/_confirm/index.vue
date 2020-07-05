<template>
    <div>
        <p>email: {{ $route.params.confirm}}</p>

    </div>
</template>
<script>
export default {
    // 페이지가 렌딩되면(?) 자동으로 호출되는 메소드
    validate(data) {
        // regex 숫자만 허용
        return /^\d+$/.test(data.params.confirm)
    }
}
</script>
