class VitalsRepository(private val dao: VitalsDao) {
    val allVitals = dao.getAllVitals()

    suspend fun insertVitals(vitals: VitalsEntity) {
        dao.insertVitals(vitals)
    }
}
