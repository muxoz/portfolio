<template>
    <div id="basic-modal" class="overlay modal overlay-open:opacity-100 hidden" role="dialog" tabindex="-1">
        <div class="modal-dialog overlay-open:opacity-100">
            <div class="modal-content">
                <div class="modal-header">
                    <h3 class="modal-title">FORMACIÓN</h3>
                    <button type="button" class="btn btn-text btn-circle btn-sm absolute end-3 top-3" aria-label="Close"
                        data-overlay="#basic-modal">
                        <span class="icon-[tabler--x] size-4"></span>
                    </button>
                </div>
                <div class="accordion divide-neutral/20 divide-y modal-body ">
                    <div class="accordion-item active" id="payment-arrow">
                        <button class="accordion-toggle inline-flex items-center gap-x-4 text-start"
                            aria-controls="payment-arrow-collapse" aria-expanded="true">
                            <span
                                class="icon-[tabler--chevron-right] accordion-item-active:rotate-90 size-5 shrink-0 transition-transform duration-300 rtl:rotate-180"></span>
                            Ingeniería de Sistemas
                        </button>
                        <div id="payment-arrow-collapse"
                            class="accordion-content w-full overflow-hidden transition-[height] duration-300"
                            aria-labelledby="payment-arrow" role="region">
                            <div class="px-5 pb-4">
                                <p class="text-base-content/80 font-normal">
                                    Universidad Nacional Abierta y a Distancia (UNAD) |  (2022 - Actualidad) <br>
                                    Estudios en progreso enfocados en el diseño, desarrollo y gestión de sistemas tecnológicos.
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item" id="delivery-arrow">
                        <button class="accordion-toggle inline-flex items-center gap-x-4 text-start"
                            aria-controls="delivery-arrow-collapse" aria-expanded="false">
                            <span
                                class="icon-[tabler--chevron-right] accordion-item-active:rotate-90 size-5 shrink-0 transition-transform duration-300 rtl:rotate-180"></span>
                            Desarrollo de Aplicaciones Web
                        </button>
                        <div id="delivery-arrow-collapse"
                            class="accordion-content hidden w-full overflow-hidden transition-[height] duration-300"
                            aria-labelledby="delivery-arrow" role="region">
                            <div class="px-5 pb-4">
                                <p class="text-base-content/80 font-normal">
                                    Universidad Tecnológica de Pereira (UTP) |  (04/2022 - 12/2022)
                                    <br>
                                    Formación especializada en la creación de aplicaciones web funcionales y escalables.
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item" id="cancel-arrow">
                        <button class="accordion-toggle inline-flex items-center gap-x-4 text-start"
                            aria-controls="cancel-arrow-collapse" aria-expanded="false">
                            <span
                                class="icon-[tabler--chevron-right] accordion-item-active:rotate-90 size-5 shrink-0 transition-transform duration-300 rtl:rotate-180"></span>
                            Desarrollo Frontend con React
                        </button>
                        <div id="cancel-arrow-collapse"
                            class="accordion-content hidden w-full overflow-hidden transition-[height] duration-300"
                            aria-labelledby="cancel-arrow" role="region">
                            <div class="px-5 pb-4">
                                <p class="text-base-content/80 font-normal">
                                    Alura | (01/2023 - 06/2023)<br>
                                    Capacitación intensiva en el desarrollo de interfaces de usuario interactivas y
                                    modernas utilizando React.
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item" id="launch">
                        <button class="accordion-toggle inline-flex items-center gap-x-4 text-start"
                            aria-controls="launch-x" aria-expanded="false">
                            <span
                                class="icon-[tabler--chevron-right] accordion-item-active:rotate-90 size-5 shrink-0 transition-transform duration-300 rtl:rotate-180"></span>
                                Desarrollo Fullstack
                               
                        </button>
                        <div id="launch-x"
                            class="accordion-content hidden w-full overflow-hidden transition-[height] duration-300"
                            aria-labelledby="launch" role="region">
                            <div class="px-5 pb-4">
                                <p class="text-base-content/80 font-normal">
                                    Launch X |  (02/2022 - 05/2022)<br>
                                    Aprendizaje práctico en tecnologías como, JavaScript, Vue.js…
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="modal-footer">
                    <button type="button" class="btn btn-soft btn-primary" data-overlay="#basic-modal">Cerrar</button>
                </div>
            </div>
        </div>
    </div>
</template>

